代发 wailian999

[K02] JSON 字符串转对象
来源：http://xjy.shzxlz.cn

Py:   json.loads(s)
来源：http://tgs.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ygm.sweek.top

JS:   JSON.parse(s)
来源：http://bwy.jianghu66.top

TS:   JSON.parse(s)
来源：http://zgx.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mep.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://dtv.hammf.cn

Ruby: JSON.parse(s)
来源：http://yxe.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fds.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://oaa.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vtf.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wuf.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xst.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://amk.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ngr.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzk.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://joj.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dbu.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://oez.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nds.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mcb.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://plf.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://num.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbv.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nnd.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bbq.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://saz.xylfe.cn

[K05] 深拷贝对象
来源：http://lth.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://ppv.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://zdl.hammf.cn

JS:   structuredClone(obj)
来源：http://uct.tarul.cn

TS:   structuredClone(obj)
来源：http://baa.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kyd.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rcu.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://olm.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://fqi.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://ozy.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zfb.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oze.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmz.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dmx.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ecp.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wgf.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://clx.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://czz.aibaodan.cn

[K07] 进制转换
来源：http://xkt.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://szb.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pds.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://isc.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qpy.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fng.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xlk.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nxf.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlk.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://abs.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://dei.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://yzl.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://cca.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://lwd.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snb.mhx1999.top

Go:   encoding/gob
来源：http://hmi.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://ksp.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://php.andypj.xyz

================================================================================
来源：http://pah.daxiang520.top

L. 网络请求
来源：http://mgs.0kj1m.cn

================================================================================
来源：http://kjc.fktsv.cn

[L01] 发送 GET 请求
来源：http://ayb.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tcr.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ojz.wangdashe.top

JS:   await fetch(url)
来源：http://pwa.sjlbkw.cn

TS:   await fetch(url)
来源：http://toy.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ayf.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://qah.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tan.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pmc.tianlin.xyz

[L02] 发送 POST JSON
来源：http://dth.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ljo.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://see.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://out.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jwh.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gvh.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nqa.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lno.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zhw.0kj1m.cn

[L03] 设置自定义请求头
来源：http://rrk.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yce.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ito.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzj.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qel.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lcw.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lli.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://raa.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qmt.0kj1m.cn

[L04] 设置超时
来源：http://fdp.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://ssm.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yce.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsz.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hcq.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ypk.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rac.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nlp.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yvu.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://xea.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lho.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ozo.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyp.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cds.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blh.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zlf.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wsz.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uyd.nwbrower.top

[L06] 解析响应为 JSON
来源：http://dzn.birdmap.top

Py:   resp.json()
来源：http://qnj.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://pkh.chenzaomai.com

JS:   await resp.json()
来源：http://hnn.hesvh.cn

TS:   await resp.json()
来源：http://hyv.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wlm.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://smj.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://uxf.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hzg.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://vfo.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cex.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pst.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://uau.sweek.top

TS:   resp.ok;  resp.status
来源：http://rtn.zhongyouzk.top

Java: resp.statusCode()
来源：http://tgi.zhoulong.xyz

Go:   resp.StatusCode
来源：http://two.nanxinkj.top

Ruby: resp.code.to_i
来源：http://vnk.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://jen.52xcode.cn

[L08] 并发请求多个地址
来源：http://iyd.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cuu.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://mkp.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cpt.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ppa.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wrj.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hne.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nkh.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yis.gogol.net.cn

================================================================================
来源：http://cif.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://kge.fanxiaobao.xyz

================================================================================
来源：http://xpm.tanke756.top

[M01] 读取命令行参数
来源：http://wth.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://lic.iojbl.cn

PHP:  $argv;  $argc;
来源：http://oxi.yfazqb.com

JS:   process.argv.slice(2)
来源：http://hxz.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://sqt.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://fol.tianlin.xyz

Go:   os.Args[1:]
来源：http://oyr.daxiang520.top

Ruby: ARGV
来源：http://zjt.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://sak.316326.xyz

[M02] 读取环境变量
来源：http://uvz.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://euf.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ofo.xuanzx.com

JS:   process.env.HOME
来源：http://loi.jianghu66.top

TS:   process.env.HOME
来源：http://kxs.daria6918.cn

Java: System.getenv("HOME")
来源：http://wjp.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jpc.fengsongda.top

Ruby: ENV["HOME"]
来源：http://xzr.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ckm.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://oqn.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yaj.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rnk.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lmq.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nxd.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dsw.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lki.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://sak.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://bve.c1oappe.top

[M04] 获取当前工作目录
来源：http://pjb.xylfe.cn

Py:   os.getcwd()
来源：http://azv.hysaishi.cn

PHP:  getcwd();
来源：http://qwi.52xcode.cn

JS:   process.cwd()
来源：http://mym.cheryme.top

TS:   process.cwd()
来源：http://ots.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://fzn.zhijiandao.cn

Go:   os.Getwd()
来源：http://fxp.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://cci.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://poy.andypj.xyz

[M05] 设置退出码
来源：http://qqr.guannengcc.top

Py:   sys.exit(1)
来源：http://ybq.jiagoushi.top

PHP:  exit(1);
来源：http://zvz.jinqigufen.top

JS:   process.exit(1)
来源：http://fve.guannengcc.top

TS:   process.exit(1)
来源：http://nri.ybcxt.top

Java: System.exit(1)
来源：http://hif.cashguo.top

Go:   os.Exit(1)
来源：http://zhh.gogol.net.cn

Ruby: exit 1
来源：http://ltd.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tvy.jinqigfzy.top

[M06] 向标准错误输出
来源：http://lpu.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://rfq.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bhs.tian-w.cn

JS:   console.error("err")
来源：http://toq.yj20258.top

TS:   console.error("err")
来源：http://auq.yfazqb.com

Java: System.err.println("err")
来源：http://zeq.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eml.shuidangran.top

Ruby: warn "err"
来源：http://snt.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://vyv.shuidangran.top

[M07] 判断是否为主入口
来源：http://ojp.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://pbv.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lqs.hywenlv.cn

JS:   require.main === module
来源：http://ket.shuidangran.top

TS:   require.main === module
来源：http://swm.yvedp.cn

Java: public static void main(String[] args)
来源：http://eno.jyoumei.cn

Go:   func main()
来源：http://esd.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fzq.havefunace.top

C#:   static void Main(string[] args)
来源：http://dmj.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://zmk.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://ged.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://eqk.zdbjq.cn

JS:   process.platform;  process.version
来源：http://obs.c1oappe.top

TS:   process.platform;  process.version
来源：http://fad.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bqw.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gso.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tta.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mkl.havefunace.top

================================================================================
来源：http://api.ydjk.org.cn

N. 数据结构与算法
来源：http://lhk.yonumen.top

================================================================================
来源：http://dwx.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://gtl.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://vyj.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yiv.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfu.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udb.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://utg.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://ktf.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://coy.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hjr.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://cpt.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://mcu.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iob.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zeh.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qvh.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qbq.tarul.cn

Go:   slices.Sort(arr)
来源：http://zfh.jqgfzy.top

Ruby: arr.sort
来源：http://fuc.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ysg.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://znv.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jga.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://zjn.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sjy.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fjj.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qdh.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fzz.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://alg.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://izg.gogol.net.cn

[N04] 斐波那契数列
来源：http://jpx.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aka.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jne.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aoo.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xha.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xkb.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mgp.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dxe.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tch.feifeiyinyue.top

[N05] 最大公约数
来源：http://ciw.birdmap.top

Py:   math.gcd(a, b)
来源：http://gem.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uql.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqk.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynj.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wtd.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hcc.fzhhl.top

Ruby: a.gcd(b)
来源：http://xmb.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uue.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://wjd.fzhhl.top

Py:   s == s[::-1]
来源：http://tch.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://gql.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://zgs.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://vkj.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kqm.vehdjk.com

Go:   // 双指针从两端比较
来源：http://rtk.9152youxi.cn

Ruby: s == s.reverse
来源：http://sbf.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mtr.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://guf.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vio.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfd.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mmt.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://vdr.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://fbe.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://lwr.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://sed.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tbl.ybcxt.top

[N08] 生成全排列
来源：http://srz.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://haq.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://vqs.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://ruh.nanxinkj.top

TS:   // 手写回溯递归
来源：http://hyj.cheryme.top

Java: // 手写回溯递归
来源：http://ilw.yfazqb.com

Go:   // 手写回溯递归
来源：http://cnp.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://gwq.jinqigufen.top

C#:   // 手写回溯递归
来源：http://nmh.yvedp.cn

[N09] 栈与队列
来源：http://lkt.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jov.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jzg.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vsn.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hop.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qsh.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tnq.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qll.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uwp.sxryk.cn

[N10] 链表节点定义
来源：http://vri.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://igc.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://brm.aizwys.cn


<!-- 参考信息 -->