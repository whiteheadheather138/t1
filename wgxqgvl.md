代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://yy.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://zy.zhonguo3118.cn

JS:   JSON.stringify(obj)
来源：https://ud.zhonguo6118.cn

TS:   JSON.stringify(obj)
来源：https://fm.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://pg.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://yb.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://kv.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://dg.zhonguo2118.cn

[K02] JSON 字符串转对象
来源：https://ui.zhonguo8118.cn

Py:   json.loads(s)
来源：https://pq.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://hc.zhonguo7118.cn

JS:   JSON.parse(s)
来源：https://xx.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://tp.zhonguo5118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://bd.zhonguo5118.cn

Go:   json.Unmarshal(data, &v)
来源：https://no.zhonguo6118.cn

Ruby: JSON.parse(s)
来源：https://qf.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://ck.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://jx.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://ys.zhonguo5118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://yu.zhonguo4118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://mf.zhonguo5118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://pk.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://wx.zhonguo8118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://ec.zhonguo4118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://nl.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://og.zhonguo4118.cn

[K04] 读取 JSON 文件
来源：https://gs.zhonguo1118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://yl.zhonguo8118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://lr.zhonguo6118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ir.zhonguo3118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://hy.zhonguo5118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://wh.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://yi.zhonguo7118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://vd.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://kt.zhonguo7118.cn

[K05] 深拷贝对象
来源：https://qf.zhonguo2118.cn

Py:   copy.deepcopy(obj)
来源：https://ze.zhonguo1118.cn

PHP:  unserialize(serialize($obj));
来源：https://ch.zhonguo2118.cn

JS:   structuredClone(obj)
来源：https://ke.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://nl.zhonguo2118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ev.zhonguo6118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://hi.zhonguo1118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://tu.zhonguo7118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://iz.zhonguo4118.cn

[K06] 解析 URL 查询串
来源：https://cx.zhonguo1118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://ri.zhonguo6118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://po.zhonguo8118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ju.zhonguo2118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://pg.zhonguo1118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://xt.zhonguo3118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://me.zhonguo1118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://ip.zhonguo7118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://pa.zhonguo8118.cn

[K07] 进制转换
来源：https://mi.zhonguo8118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ut.zhonguo1118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://kr.zhonguo7118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://iw.zhonguo6118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://wa.zhonguo1118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://sc.zhonguo7118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://eh.zhonguo8118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://rm.zhonguo7118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://ew.zhonguo7118.cn

[K08] 二进制序列化（非 JSON）
来源：https://os.zhonguo7118.cn

Py:   pickle.dumps(obj)
来源：https://or.zhonguo2118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://kp.zhonguo4118.cn

JS:   v8.serialize(obj)        // Node
来源：https://nz.zhonguo5118.cn

TS:   v8.serialize(obj)        // Node
来源：https://pn.zhonguo8118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://ne.zhonguo3118.cn

Go:   encoding/gob
来源：https://ct.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://fz.zhonguo6118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://rd.zhonguo2118.cn

================================================================================
来源：https://rs.zhonguo2118.cn

L. 网络请求
来源：https://xt.zhonguo6118.cn

================================================================================
来源：https://pw.zhonguo4118.cn

[L01] 发送 GET 请求
来源：https://ht.zhonguo1118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://ls.zhonguo6118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://jf.zhonguo3118.cn

JS:   await fetch(url)
来源：https://wl.zhonguo2118.cn

TS:   await fetch(url)
来源：https://tv.zhonguo2118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://qe.zhonguo4118.cn

Go:   resp, err := http.Get(url)
来源：https://id.zhonguo8118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://vj.zhonguo7118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://ag.zhonguo8118.cn

[L02] 发送 POST JSON
来源：https://zt.zhonguo5118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://kk.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://ab.zhonguo4118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://nu.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://qq.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://bm.zhonguo5118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://gw.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://tj.zhonguo5118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://ru.zhonguo2118.cn

[L03] 设置自定义请求头
来源：https://jr.zhonguo4118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://he.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://jb.zhonguo2118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://dq.zhonguo6118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://sn.zhonguo7118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://nl.zhonguo6118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://np.zhonguo4118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://lw.zhonguo3118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://mc.zhonguo7118.cn

[L04] 设置超时
来源：https://pw.zhonguo8118.cn

Py:   requests.get(url, timeout=5)
来源：https://ca.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://by.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ko.zhonguo3118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://sw.zhonguo7118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://wz.zhonguo4118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://ts.zhonguo5118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://ur.zhonguo1118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://xp.zhonguo6118.cn

[L05] 上传文件（multipart）
来源：https://cj.zhonguo3118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://bf.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://gk.zhonguo7118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://ph.zhonguo3118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://fo.zhonguo3118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://ag.zhonguo2118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://vt.zhonguo8118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://yc.zhonguo5118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://ex.zhonguo8118.cn

[L06] 解析响应为 JSON
来源：https://fw.zhonguo5118.cn

Py:   resp.json()
来源：https://yc.zhonguo7118.cn

PHP:  json_decode($body, true);
来源：https://vc.zhonguo3118.cn

JS:   await resp.json()
来源：https://fc.zhonguo2118.cn

TS:   await resp.json()
来源：https://ry.zhonguo3118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://km.zhonguo7118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://ah.zhonguo6118.cn

Ruby: JSON.parse(resp.body)
来源：https://ty.zhonguo4118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://pz.zhonguo5118.cn

[L07] 处理 HTTP 状态码
来源：https://gd.zhonguo8118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://cf.zhonguo2118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://oq.zhonguo3118.cn

JS:   resp.ok;  resp.status
来源：https://tx.zhonguo5118.cn

TS:   resp.ok;  resp.status
来源：https://dp.zhonguo5118.cn

Java: resp.statusCode()
来源：https://ac.zhonguo6118.cn

Go:   resp.StatusCode
来源：https://ad.zhonguo6118.cn

Ruby: resp.code.to_i
来源：https://pi.zhonguo7118.cn

C#:   (int)resp.StatusCode
来源：https://ls.zhonguo5118.cn

[L08] 并发请求多个地址
来源：https://yx.zhonguo5118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://yw.zhonguo7118.cn

PHP:  curl_multi_init() 系列
来源：https://ho.zhonguo5118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://we.zhonguo4118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://qj.zhonguo8118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://lk.zhonguo3118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://tq.zhonguo3118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://sh.zhonguo7118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://fh.zhonguo7118.cn

================================================================================
来源：https://wm.zhonguo1118.cn

M. 命令行 / 进程 / 环境
来源：https://dp.zhonguo4118.cn

================================================================================
来源：https://sc.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://ik.zhonguo6118.cn

Py:   sys.argv[1:]
来源：https://kt.zhonguo5118.cn

PHP:  $argv;  $argc;
来源：https://qh.zhonguo8118.cn

JS:   process.argv.slice(2)
来源：https://in.zhonguo4118.cn

TS:   process.argv.slice(2)
来源：https://vo.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://iy.zhonguo7118.cn

Go:   os.Args[1:]
来源：https://ru.zhonguo5118.cn

Ruby: ARGV
来源：https://hf.zhonguo4118.cn

C#:   args 数组（Main 方法参数）
来源：https://vb.zhonguo2118.cn

[M02] 读取环境变量
来源：https://of.zhonguo4118.cn

Py:   os.environ.get("HOME")
来源：https://gc.zhonguo4118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://qc.zhonguo7118.cn

JS:   process.env.HOME
来源：https://ch.zhonguo3118.cn

TS:   process.env.HOME
来源：https://fg.zhonguo4118.cn

Java: System.getenv("HOME")
来源：https://ex.zhonguo2118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://gk.zhonguo4118.cn

Ruby: ENV["HOME"]
来源：https://tn.zhonguo6118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://zm.zhonguo3118.cn

[M03] 执行外部命令
来源：https://wy.zhonguo7118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://kn.zhonguo6118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://wr.zhonguo3118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://ac.zhonguo3118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://qs.zhonguo1118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://nl.zhonguo4118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://sa.zhonguo4118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://cj.zhonguo6118.cn

C#:   Process.Start("ls", "-l");
来源：https://ov.zhonguo2118.cn

[M04] 获取当前工作目录
来源：https://ot.zhonguo1118.cn

Py:   os.getcwd()
来源：https://tk.zhonguo7118.cn

PHP:  getcwd();
来源：https://mt.zhonguo2118.cn

JS:   process.cwd()
来源：https://zv.zhonguo2118.cn

TS:   process.cwd()
来源：https://bz.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://aj.zhonguo3118.cn

Go:   os.Getwd()
来源：https://jk.zhonguo5118.cn

Ruby: Dir.pwd
来源：https://lq.zhonguo7118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ey.zhonguo8118.cn

[M05] 设置退出码
来源：https://wf.zhonguo3118.cn

Py:   sys.exit(1)
来源：https://ve.zhonguo3118.cn

PHP:  exit(1);
来源：https://ox.zhonguo5118.cn

JS:   process.exit(1)
来源：https://qj.zhonguo8118.cn

TS:   process.exit(1)
来源：https://ed.zhonguo2118.cn

Java: System.exit(1)
来源：https://qv.zhonguo4118.cn

Go:   os.Exit(1)
来源：https://wf.zhonguo6118.cn

Ruby: exit 1
来源：https://ls.zhonguo6118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://vd.zhonguo5118.cn

[M06] 向标准错误输出
来源：https://gf.zhonguo7118.cn

Py:   print("err", file=sys.stderr)
来源：https://dn.zhonguo6118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://vs.zhonguo5118.cn

JS:   console.error("err")
来源：https://ms.zhonguo8118.cn

TS:   console.error("err")
来源：https://qz.zhonguo4118.cn

Java: System.err.println("err")
来源：https://cy.zhonguo4118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://id.zhonguo6118.cn

Ruby: warn "err"
来源：https://nv.zhonguo6118.cn

C#:   Console.Error.WriteLine("err")
来源：https://tu.zhonguo1118.cn

[M07] 判断是否为主入口
来源：https://qg.zhonguo8118.cn

Py:   if __name__ == "__main__":
来源：https://ag.zhonguo8118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://fr.zhonguo2118.cn

JS:   require.main === module
来源：https://cg.zhonguo1118.cn

TS:   require.main === module
来源：https://po.zhonguo2118.cn

Java: public static void main(String[] args)
来源：https://ee.zhonguo4118.cn

Go:   func main()
来源：https://lu.zhonguo2118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://xn.zhonguo8118.cn

C#:   static void Main(string[] args)
来源：https://ri.zhonguo5118.cn

[M08] 获取系统与运行时信息
来源：https://hy.zhonguo8118.cn

Py:   platform.system();  platform.python_version()
来源：https://eb.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://jf.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://xj.zhonguo3118.cn

TS:   process.platform;  process.version
来源：https://tw.zhonguo3118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://iq.zhonguo5118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://cx.zhonguo8118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://mw.zhonguo8118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://ty.zhonguo8118.cn

================================================================================
来源：https://ka.zhonguo5118.cn

N. 数据结构与算法
来源：https://yi.zhonguo7118.cn

================================================================================
来源：https://aa.zhonguo7118.cn

[N01] 二分查找（有序数组）
来源：https://cd.zhonguo8118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://ym.zhonguo6118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://qt.zhonguo3118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://br.zhonguo6118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://um.zhonguo8118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://jk.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://mb.zhonguo7118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://wy.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://kn.zhonguo5118.cn

[N02] 排序（工程实践用内置实现）
来源：https://fq.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://xq.zhonguo8118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ct.zhonguo8118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://dx.zhonguo4118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://mf.zhonguo8118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://sr.zhonguo3118.cn

Go:   slices.Sort(arr)
来源：https://kh.zhonguo3118.cn

Ruby: arr.sort
来源：https://lt.zhonguo3118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://xb.zhonguo7118.cn

[N03] 快速排序（分治示例）
来源：https://cw.zhonguo2118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://ud.zhonguo8118.cn

PHP:  // 递归实现，或用 usort
来源：https://pd.zhonguo7118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://mc.zhonguo5118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://pu.zhonguo6118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://es.zhonguo4118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://tg.zhonguo4118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://qk.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://pj.zhonguo7118.cn

[N04] 斐波那契数列
来源：https://cd.zhonguo6118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://jw.zhonguo6118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://xj.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://yq.zhonguo5118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ba.zhonguo2118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://lr.zhonguo2118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://iq.zhonguo4118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://em.zhonguo8118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://sb.zhonguo7118.cn

[N05] 最大公约数
来源：https://yv.zhonguo5118.cn

Py:   math.gcd(a, b)
来源：https://gu.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://ic.zhonguo1118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://ux.zhonguo2118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://bl.zhonguo3118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://eo.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://ja.zhonguo3118.cn

Ruby: a.gcd(b)
来源：https://nw.zhonguo3118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://zp.zhonguo5118.cn

[N06] 判断回文字符串
来源：https://ua.zhonguo7118.cn

Py:   s == s[::-1]
来源：https://jx.zhonguo5118.cn

PHP:  $s === strrev($s);
来源：https://ci.zhonguo1118.cn

JS:   s === [...s].reverse().join("")
来源：https://cw.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://zp.zhonguo6118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://fl.zhonguo1118.cn

Go:   // 双指针从两端比较
来源：https://nf.zhonguo6118.cn

Ruby: s == s.reverse
来源：https://oh.zhonguo8118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://mz.zhonguo6118.cn

[N07] 两数之和（返回下标）
来源：https://sg.zhonguo4118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://ar.zhonguo7118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://up.zhonguo5118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://pq.zhonguo5118.cn

TS:   // 手写 Map<string, number>
来源：https://vz.zhonguo8118.cn

Java: // 手写 HashMap
来源：https://ft.zhonguo1118.cn

Go:   // 手写 map[int]int
来源：https://ep.zhonguo2118.cn

Ruby: // 手写 Hash
来源：https://au.zhonguo4118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://nx.zhonguo4118.cn

[N08] 生成全排列
来源：https://ex.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://yj.zhonguo5118.cn

PHP:  // 手写递归交换
来源：https://sk.zhonguo1118.cn

JS:   // 手写回溯递归
来源：https://yg.zhonguo3118.cn

TS:   // 手写回溯递归
来源：https://if.zhonguo4118.cn

Java: // 手写回溯递归
来源：https://ts.zhonguo1118.cn

Go:   // 手写回溯递归
来源：https://io.zhonguo8118.cn

Ruby: arr.permutation.to_a
来源：https://ew.zhonguo3118.cn

C#:   // 手写回溯递归
来源：https://fc.zhonguo4118.cn

[N09] 栈与队列
来源：https://ky.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://ru.zhonguo5118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://wm.zhonguo4118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://eu.zhonguo8118.cn


<!-- 参考信息 -->