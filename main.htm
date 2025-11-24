import React, { useState } from 'react';
import { Search, Ticket, LogOut } from 'lucide-react';

export default function TicketSystem() {
  const [page, setPage] = useState('login');
  const [username, setUsername] = useState('');
  const [password, setPassword] = useState('');
  const [error, setError] = useState('');
  const [currentTicket, setCurrentTicket] = useState(null);
  const [searchId, setSearchId] = useState('');
  const [searchResult, setSearchResult] = useState(null);
  
  // Ticket form state
  const [description, setDescription] = useState('');
  const [country, setCountry] = useState('');
  const [phoneNumber, setPhoneNumber] = useState('');
  const [emergency, setEmergency] = useState('');
  
  // Store tickets in memory
  const [tickets, setTickets] = useState({});

  const handleLogin = (e) => {
    e.preventDefault();
    if (username === 'user1' && password === 'Password123') {
      setError('');
      setPage('form');
    } else {
      setError('Invalid username or password');
    }
  };

  const handleLogout = () => {
    setUsername('');
    setPassword('');
    setPage('login');
    setError('');
  };

  const generateTicketId = () => {
    return 'TKT-' + Date.now() + '-' + Math.floor(Math.random() * 1000);
  };

  const getTodayDate = () => {
    return new Date().toISOString().split('T')[0];
  };

  const handleSubmitTicket = (e) => {
    e.preventDefault();
    
    if (!description.trim()) {
      alert('Please enter a description');
      return;
    }
    
    if (!country) {
      alert('Please select a country');
      return;
    }
    
    if (!phoneNumber.trim()) {
      alert('Please enter a phone number');
      return;
    }
    
    if (!emergency) {
      alert('Please select emergency status (Yes or No)');
      return;
    }

    const ticketId = generateTicketId();
    const newTicket = {
      id: ticketId,
      description,
      country,
      dateRequest: getTodayDate(),
      phoneNumber,
      emergency,
      status: 'Open',
      createdAt: new Date().toLocaleString()
    };

    setTickets(prev => ({...prev, [ticketId]: newTicket}));
    setCurrentTicket(newTicket);
    
    // Reset form
    setDescription('');
    setCountry('');
    setPhoneNumber('');
    setEmergency('');
    
    setPage('success');
  };

  const handleSearch = (e) => {
    e.preventDefault();
    const ticket = tickets[searchId];
    if (ticket) {
      setSearchResult(ticket);
    } else {
      setSearchResult({ notFound: true });
    }
  };

  const countries = [
    'United States', 'HongKong', 'Canada', 'Australia', 'Germany',
    'France', 'Japan', 'Singapore', 'Malaysia', 'Taiwan', 'China'
  ];

  // Login Page
  if (page === 'login') {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 flex items-center justify-center p-4">
        <div className="bg-white rounded-lg shadow-xl p-8 w-full max-w-md">
          <div className="flex items-center justify-center mb-6">
            <Ticket className="w-12 h-12 text-indigo-600" />
          </div>
          <h1 className="text-3xl font-bold text-center text-gray-800 mb-8">Ticket System</h1>
          
          <div>
            <div className="mb-4">
              <label className="block text-gray-700 text-sm font-semibold mb-2">
                Username
              </label>
              <input
                type="text"
                value={username}
                onChange={(e) => setUsername(e.target.value)}
                className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                placeholder="Enter username"
              />
            </div>
            
            <div className="mb-6">
              <label className="block text-gray-700 text-sm font-semibold mb-2">
                Password
              </label>
              <input
                type="password"
                value={password}
                onChange={(e) => setPassword(e.target.value)}
                onKeyPress={(e) => e.key === 'Enter' && handleLogin(e)}
                className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                placeholder="Enter password"
              />
            </div>
            
            {error && (
              <div className="mb-4 p-3 bg-red-100 border border-red-400 text-red-700 rounded-lg text-sm">
                {error}
              </div>
            )}
            
            <button
              onClick={handleLogin}
              className="w-full bg-indigo-600 text-white py-2 px-4 rounded-lg hover:bg-indigo-700 transition duration-200 font-semibold"
            >
              Login
            </button>
          </div>
          
          <div className="mt-4 text-center text-sm text-gray-600">
            <p>Demo credentials:</p>
            //<p className="font-mono">user1 / 123</p>
          </div>
        </div>
      </div>
    );
  }

  // Ticket Form Page
  if (page === 'form') {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 p-4">
        <div className="max-w-4xl mx-auto">
          <div className="bg-white rounded-lg shadow-xl p-8 mb-6">
            <div className="flex justify-between items-center mb-6">
              <h1 className="text-3xl font-bold text-gray-800">Create New Ticket</h1>
              <div className="flex gap-2">
                <button
                  onClick={() => setPage('allTickets')}
                  className="flex items-center gap-2 px-4 py-2 bg-indigo-600 hover:bg-indigo-700 text-white rounded-lg transition"
                >
                  <Ticket className="w-4 h-4" />
                  View All Tickets
                </button>
                <button
                  onClick={handleLogout}
                  className="flex items-center gap-2 px-4 py-2 bg-gray-200 hover:bg-gray-300 rounded-lg transition"
                >
                  <LogOut className="w-4 h-4" />
                  Logout
                </button>
              </div>
            </div>
            
            <div>
              <div className="mb-4">
                <label className="block text-gray-700 text-sm font-semibold mb-2">
                  Description *
                </label>
                <textarea
                  value={description}
                  onChange={(e) => setDescription(e.target.value)}
                  className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                  rows="4"
                  placeholder="Describe your issue..."
                />
              </div>
              
              <div className="mb-4">
                <label className="block text-gray-700 text-sm font-semibold mb-2">
                  Country *
                </label>
                <select
                  value={country}
                  onChange={(e) => setCountry(e.target.value)}
                  className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                >
                  <option value="">Select a country</option>
                  {countries.map(c => (
                    <option key={c} value={c}>{c}</option>
                  ))}
                </select>
              </div>
              
              <div className="mb-4">
                <label className="block text-gray-700 text-sm font-semibold mb-2">
                  Date Request
                </label>
                <input
                  type="text"
                  value={getTodayDate()}
                  className="w-full px-4 py-2 border border-gray-300 rounded-lg bg-gray-50"
                  disabled
                />
              </div>
              
              <div className="mb-4">
                <label className="block text-gray-700 text-sm font-semibold mb-2">
                  Phone Number *
                </label>
                <input
                  type="tel"
                  value={phoneNumber}
                  onChange={(e) => setPhoneNumber(e.target.value)}
                  className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                  placeholder="+1234567890"
                />
              </div>
              
              <div className="mb-6">
                <label className="block text-gray-700 text-sm font-semibold mb-3">
                  Emergency *
                </label>
                <div className="flex gap-6">
                  <label className="flex items-center gap-2 cursor-pointer">
                    <input
                      type="checkbox"
                      checked={emergency === 'Yes'}
                      onChange={(e) => setEmergency(e.target.checked ? 'Yes' : '')}
                      className="w-5 h-5 text-indigo-600 border-gray-300 rounded focus:ring-2 focus:ring-indigo-500"
                    />
                    <span className="text-gray-700 text-sm font-semibold">
                      Yes
                    </span>
                  </label>
                  <label className="flex items-center gap-2 cursor-pointer">
                    <input
                      type="checkbox"
                      checked={emergency === 'No'}
                      onChange={(e) => setEmergency(e.target.checked ? 'No' : '')}
                      className="w-5 h-5 text-indigo-600 border-gray-300 rounded focus:ring-2 focus:ring-indigo-500"
                    />
                    <span className="text-gray-700 text-sm font-semibold">
                      No
                    </span>
                  </label>
                </div>
              </div>
              
              <button
                onClick={handleSubmitTicket}
                className="w-full bg-indigo-600 text-white py-3 px-4 rounded-lg hover:bg-indigo-700 transition duration-200 font-semibold"
              >
                Submit Ticket
              </button>
            </div>
          </div>
          
          {/* Search Section */}
          <div className="bg-white rounded-lg shadow-xl p-8">
            <h2 className="text-2xl font-bold text-gray-800 mb-4">Search Ticket</h2>
            <div className="flex gap-2 mb-4">
              <input
                type="text"
                value={searchId}
                onChange={(e) => setSearchId(e.target.value)}
                onKeyPress={(e) => e.key === 'Enter' && handleSearch(e)}
                className="flex-1 px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-500"
                placeholder="Enter Ticket ID (e.g., TKT-123456-789)"
              />
              <button
                onClick={handleSearch}
                className="px-6 py-2 bg-green-600 text-white rounded-lg hover:bg-green-700 transition flex items-center gap-2"
              >
                <Search className="w-4 h-4" />
                Search
              </button>
            </div>
            
            {searchResult && (
              <div className="mt-4 p-4 border border-gray-300 rounded-lg">
                {searchResult.notFound ? (
                  <p className="text-red-600 font-semibold">Ticket not found</p>
                ) : (
                  <div>
                    <h3 className="font-bold text-lg mb-2">Ticket Details</h3>
                    <div className="grid grid-cols-2 gap-2 text-sm">
                      <p><span className="font-semibold">ID:</span> {searchResult.id}</p>
                      <p><span className="font-semibold">Status:</span> 
                        <span className="ml-2 px-2 py-1 bg-green-100 text-green-800 rounded">
                          {searchResult.status}
                        </span>
                      </p>
                      <p><span className="font-semibold">Country:</span> {searchResult.country}</p>
                      <p><span className="font-semibold">Phone:</span> {searchResult.phoneNumber}</p>
                      <p><span className="font-semibold">Emergency:</span> 
                        <span className={`ml-2 px-2 py-1 rounded text-xs font-semibold ${
                          searchResult.emergency === 'Yes' 
                            ? 'bg-red-100 text-red-800' 
                            : 'bg-gray-100 text-gray-800'
                        }`}>
                          {searchResult.emergency}
                        </span>
                      </p>
                      <p className="col-span-2"><span className="font-semibold">Description:</span> {searchResult.description}</p>
                      <p><span className="font-semibold">Date:</span> {searchResult.dateRequest}</p>
                      <p><span className="font-semibold">Created:</span> {searchResult.createdAt}</p>
                    </div>
                  </div>
                )}
              </div>
            )}
          </div>
        </div>
      </div>
    );
  }

  // All Tickets Page
  if (page === 'allTickets') {
    const ticketArray = Object.values(tickets);
    
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 p-4">
        <div className="max-w-7xl mx-auto">
          <div className="bg-white rounded-lg shadow-xl p-8">
            <div className="flex justify-between items-center mb-6">
              <h1 className="text-3xl font-bold text-gray-800">All Tickets</h1>
              <div className="flex gap-2">
                <button
                  onClick={() => setPage('form')}
                  className="px-4 py-2 bg-indigo-600 hover:bg-indigo-700 text-white rounded-lg transition"
                >
                  Create Ticket
                </button>
                <button
                  onClick={handleLogout}
                  className="flex items-center gap-2 px-4 py-2 bg-gray-200 hover:bg-gray-300 rounded-lg transition"
                >
                  <LogOut className="w-4 h-4" />
                  Logout
                </button>
              </div>
            </div>
            
            {ticketArray.length === 0 ? (
              <div className="text-center py-12">
                <Ticket className="w-16 h-16 text-gray-300 mx-auto mb-4" />
                <p className="text-gray-500 text-lg">No tickets created yet</p>
                <button
                  onClick={() => setPage('form')}
                  className="mt-4 px-6 py-2 bg-indigo-600 hover:bg-indigo-700 text-white rounded-lg transition"
                >
                  Create Your First Ticket
                </button>
              </div>
            ) : (
              <div className="overflow-x-auto">
                <table className="w-full border-collapse">
                  <thead>
                    <tr className="bg-gray-100 border-b-2 border-gray-300">
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Ticket ID</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Description</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Country</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Phone</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Date</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Emergency</th>
                      <th className="px-4 py-3 text-left text-sm font-semibold text-gray-700">Status</th>
                    </tr>
                  </thead>
                  <tbody>
                    {ticketArray.map((ticket, index) => (
                      <tr 
                        key={ticket.id} 
                        className={`border-b hover:bg-gray-50 ${index % 2 === 0 ? 'bg-white' : 'bg-gray-50'}`}
                      >
                        <td className="px-4 py-3 text-sm font-mono text-indigo-600">{ticket.id}</td>
                        <td className="px-4 py-3 text-sm text-gray-700 max-w-xs truncate" title={ticket.description}>
                          {ticket.description}
                        </td>
                        <td className="px-4 py-3 text-sm text-gray-700">{ticket.country}</td>
                        <td className="px-4 py-3 text-sm text-gray-700">{ticket.phoneNumber}</td>
                        <td className="px-4 py-3 text-sm text-gray-700">{ticket.dateRequest}</td>
                        <td className="px-4 py-3 text-sm">
                          <span className={`px-2 py-1 rounded text-xs font-semibold ${
                            ticket.emergency === 'Yes' 
                              ? 'bg-red-100 text-red-800' 
                              : 'bg-gray-100 text-gray-800'
                          }`}>
                            {ticket.emergency}
                          </span>
                        </td>
                        <td className="px-4 py-3 text-sm">
                          <span className="px-2 py-1 bg-green-100 text-green-800 rounded text-xs font-semibold">
                            {ticket.status}
                          </span>
                        </td>
                      </tr>
                    ))}
                  </tbody>
                </table>
                
                <div className="mt-4 text-sm text-gray-600">
                  Total Tickets: <span className="font-semibold">{ticketArray.length}</span>
                </div>
              </div>
            )}
          </div>
        </div>
      </div>
    );
  }

  // Success Page
  if (page === 'success') {
    return (
      <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 flex items-center justify-center p-4">
        <div className="bg-white rounded-lg shadow-xl p-8 w-full max-w-2xl">
          <div className="text-center mb-6">
            <div className="inline-flex items-center justify-center w-16 h-16 bg-green-100 rounded-full mb-4">
              <svg className="w-8 h-8 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M5 13l4 4L19 7" />
              </svg>
            </div>
            <h1 className="text-3xl font-bold text-gray-800 mb-2">Ticket Created Successfully!</h1>
            <p className="text-gray-600">Your ticket has been submitted and is being processed.</p>
          </div>
          
          <div className="bg-gray-50 rounded-lg p-6 mb-6">
            <h2 className="text-xl font-bold text-gray-800 mb-4">Ticket Details</h2>
            <div className="space-y-2 text-sm">
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Ticket ID:</span>
                <span className="font-mono text-indigo-600">{currentTicket?.id}</span>
              </div>
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Status:</span>
                <span className="px-2 py-1 bg-green-100 text-green-800 rounded text-xs font-semibold">
                  {currentTicket?.status}
                </span>
              </div>
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Country:</span>
                <span>{currentTicket?.country}</span>
              </div>
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Date:</span>
                <span>{currentTicket?.dateRequest}</span>
              </div>
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Phone:</span>
                <span>{currentTicket?.phoneNumber}</span>
              </div>
              <div className="flex justify-between">
                <span className="font-semibold text-gray-700">Emergency:</span>
                <span className={`px-2 py-1 rounded text-xs font-semibold ${
                  currentTicket?.emergency === 'Yes' 
                    ? 'bg-red-100 text-red-800' 
                    : 'bg-gray-100 text-gray-800'
                }`}>
                  {currentTicket?.emergency}
                </span>
              </div>
              <div className="pt-2 border-t">
                <span className="font-semibold text-gray-700">Description:</span>
                <p className="mt-1 text-gray-600">{currentTicket?.description}</p>
              </div>
            </div>
          </div>
          
          <div className="flex gap-4">
            <button
              onClick={() => setPage('form')}
              className="flex-1 bg-indigo-600 text-white py-3 px-4 rounded-lg hover:bg-indigo-700 transition font-semibold"
            >
              Create Another Ticket
            </button>
            <button
              onClick={handleLogout}
              className="px-6 py-3 bg-gray-200 text-gray-700 rounded-lg hover:bg-gray-300 transition font-semibold"
            >
              Logout
            </button>
          </div>
        </div>
      </div>
    );
  }
}
