
export default function TravelInquirySite() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-pink-50 to-white text-gray-800 p-6">
      <div className="max-w-4xl mx-auto">
        <div className="text-center mb-10">
          <h1 className="text-5xl font-bold mb-4">AT Pretty Adventures</h1>
          <p className="text-lg text-gray-600">
            Let me help you plan the vacation of your dreams ✈️
          </p>
        </div>

        <div className="bg-white shadow-2xl rounded-3xl p-8 border border-pink-100">
          <h2 className="text-3xl font-semibold mb-6 text-center">
            Travel Planning Form
          </h2>

          <form className="space-y-6">
            <div className="grid md:grid-cols-2 gap-6">
              <div>
                <label className="block mb-2 font-medium">Full Name</label>
                <input
                  type="text"
                  placeholder="Your full name"
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>

              <div>
                <label className="block mb-2 font-medium">Email Address</label>
                <input
                  type="email"
                  placeholder="example@email.com"
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>
            </div>

            <div className="grid md:grid-cols-2 gap-6">
              <div>
                <label className="block mb-2 font-medium">Phone Number</label>
                <input
                  type="tel"
                  placeholder="(123) 456-7890"
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>

              <div>
                <label className="block mb-2 font-medium">Desired Destination</label>
                <input
                  type="text"
                  placeholder="Disney, Hawaii, Cancun..."
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>
            </div>

            <div className="grid md:grid-cols-2 gap-6">
              <div>
                <label className="block mb-2 font-medium">Approximate Travel Date</label>
                <input
                  type="date"
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>

              <div>
                <label className="block mb-2 font-medium">How Many Travelers?</label>
                <input
                  type="number"
                  placeholder="2"
                  className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
                />
              </div>
            </div>

            <div>
              <label className="block mb-2 font-medium">What Type of Trip Are You Looking For?</label>
              <select className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300">
                <option>Select an option</option>
                <option>Family Vacation</option>
                <option>Honeymoon</option>
                <option>Disney / Theme Parks</option>
                <option>Cruise</option>
                <option>Friends Trip</option>
                <option>All-Inclusive Resort</option>
              </select>
            </div>

            <div>
              <label className="block mb-2 font-medium">Approximate Budget</label>
              <input
                type="text"
                placeholder="$2,000 - $5,000"
                className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
              />
            </div>

            <div>
              <label className="block mb-2 font-medium">What Would You Like Help Booking?</label>
              <div className="grid md:grid-cols-2 gap-3 mt-2">
                {[
                  'Flights',
                  'Hotel',
                  'Vacation Package',
                  'Cruise',
                  'Theme Park Tickets',
                  'Transportation',
                ].map((item) => (
                  <label key={item} className="flex items-center gap-2 border rounded-2xl p-3 hover:bg-pink-50 cursor-pointer">
                    <input type="checkbox" />
                    {item}
                  </label>
                ))}
              </div>
            </div>

            <div>
              <label className="block mb-2 font-medium">Tell Me More About Your Dream Trip</label>
              <textarea
                rows="5"
                placeholder="Example: I want to visit Disney with my kids and need help with hotel and park tickets."
                className="w-full border border-gray-300 rounded-2xl p-3 focus:outline-none focus:ring-2 focus:ring-pink-300"
              ></textarea>
            </div>

            <div className="text-center pt-4">
              <button
                type="submit"
                className="bg-pink-500 hover:bg-pink-600 text-white px-8 py-4 rounded-2xl text-lg font-semibold shadow-lg transition"
              >
                Submit Information ✨
              </button>
            </div>
          </form>
        </div>

        <div className="text-center mt-10 text-gray-500">
          <p>Instagram: @prettyadventuresbyat</p>
          <p>TikTok: @tuviajerapreferida</p>
          <p>Email: travelswithaley@hotmail.com</p>
        </div>
      </div>
    </div>
  )
}
