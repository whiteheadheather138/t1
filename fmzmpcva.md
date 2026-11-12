代发 wailian999

TS:   JSON.parse(s)
来源：http://cqn.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://smb.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://cpd.316326.xyz

Ruby: JSON.parse(s)
来源：http://jda.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wjy.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://nti.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yny.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://isr.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xvr.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qge.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fub.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kzu.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hwt.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ybq.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://gyp.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uhb.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pmw.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inv.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umu.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wul.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://som.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://arz.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lsz.dianchejie.cn

[K05] 深拷贝对象
来源：http://wjr.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://iva.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://agj.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://urb.cdnleiting.top

TS:   structuredClone(obj)
来源：http://lsm.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eqc.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cda.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wlr.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ocg.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://eaj.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svy.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://flg.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://azb.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://peh.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnm.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://alu.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fhj.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zsg.jqgfzy.top

[K07] 进制转换
来源：http://bie.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pkh.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cjg.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dba.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://icq.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ecu.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bwb.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wdi.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xta.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://gzf.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://xoq.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://duu.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://kkk.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://yaw.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bdx.birdmap.top

Go:   encoding/gob
来源：http://lkb.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://uhv.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ein.shuidangran.top

================================================================================
来源：http://vwf.redwolf501.top

L. 网络请求
来源：http://zwj.shanyushiyangkeji.top

================================================================================
来源：http://cvz.cqqwz.cn

[L01] 发送 GET 请求
来源：http://txx.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hve.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pvg.shzxlz.cn

JS:   await fetch(url)
来源：http://xod.shzxlz.cn

TS:   await fetch(url)
来源：http://lly.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dvz.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://yvi.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uyn.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jid.yuxming.cn

[L02] 发送 POST JSON
来源：http://njv.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://ycb.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kck.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://smm.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcn.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nyl.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ywk.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lau.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rgq.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://ide.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ipe.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://enj.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mts.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://heg.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dsm.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eps.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lgq.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hem.jianghu66.top

[L04] 设置超时
来源：http://lwb.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://yzx.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bhq.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bqw.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hba.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jtm.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jfj.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mwr.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qrf.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://nfa.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yrb.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qyw.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfy.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lmi.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mkm.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nob.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jat.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ynd.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://sdn.cucudq.cn

Py:   resp.json()
来源：http://xxl.iojbl.cn

PHP:  json_decode($body, true);
来源：http://wcc.tanke756.top

JS:   await resp.json()
来源：http://zvc.nwbrower.top

TS:   await resp.json()
来源：http://qat.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rtu.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xzm.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://nbd.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pqr.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://hqa.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pfe.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uwh.ivvv.top

JS:   resp.ok;  resp.status
来源：http://gwm.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://jub.fengsongda.top

Java: resp.statusCode()
来源：http://fex.quarkkingdee.top

Go:   resp.StatusCode
来源：http://zwh.yuxming.cn

Ruby: resp.code.to_i
来源：http://rtm.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://viu.zhengqikj.top

[L08] 并发请求多个地址
来源：http://vrk.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nus.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://apx.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ini.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fcj.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjt.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oco.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yrs.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qdp.jianghu66.top

================================================================================
来源：http://vzu.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://lod.andypj.xyz

================================================================================
来源：http://mmf.sufxvd.cn

[M01] 读取命令行参数
来源：http://uie.c1oappe.top

Py:   sys.argv[1:]
来源：http://udc.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://neo.hammf.cn

JS:   process.argv.slice(2)
来源：http://jtv.sxryk.cn

TS:   process.argv.slice(2)
来源：http://utw.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://scj.yfazqb.com

Go:   os.Args[1:]
来源：http://sjq.gotoacloud.top

Ruby: ARGV
来源：http://tvz.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://rjr.sxryk.cn

[M02] 读取环境变量
来源：http://boy.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://ayw.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwa.yonumen.top

JS:   process.env.HOME
来源：http://jht.wangdashe.top

TS:   process.env.HOME
来源：http://whh.zhengqikj.top

Java: System.getenv("HOME")
来源：http://kgz.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wrx.daxiang520.top

Ruby: ENV["HOME"]
来源：http://urk.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xor.vehdjk.com

[M03] 执行外部命令
来源：http://vtu.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bvk.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uiu.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vwj.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://adl.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uxs.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dzo.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://oyo.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://xep.yj202588.top

[M04] 获取当前工作目录
来源：http://yip.ybcxt.top

Py:   os.getcwd()
来源：http://tsp.cqqwz.cn

PHP:  getcwd();
来源：http://ids.daria6918.cn

JS:   process.cwd()
来源：http://bcg.jlsjyb.cn

TS:   process.cwd()
来源：http://yzt.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://leh.bjfxy.top

Go:   os.Getwd()
来源：http://hdf.yonumen.top

Ruby: Dir.pwd
来源：http://viz.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gve.epnwcf.com

[M05] 设置退出码
来源：http://pgy.meibo888.top

Py:   sys.exit(1)
来源：http://smx.yj202588.top

PHP:  exit(1);
来源：http://oui.zhiwuduotai.top

JS:   process.exit(1)
来源：http://eyj.yanxiufei.cn

TS:   process.exit(1)
来源：http://luo.chenlongwang.top

Java: System.exit(1)
来源：http://mnj.ydzc1.top

Go:   os.Exit(1)
来源：http://mgn.zycfv.cn

Ruby: exit 1
来源：http://tsu.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zrv.nwbrower.top

[M06] 向标准错误输出
来源：http://oyj.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://anh.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ozk.jianghu66.top

JS:   console.error("err")
来源：http://lkz.zhoulong.xyz

TS:   console.error("err")
来源：http://nkp.fktsv.cn

Java: System.err.println("err")
来源：http://lgv.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wji.dashuyun.cn

Ruby: warn "err"
来源：http://sih.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://mrj.daria6918.cn

[M07] 判断是否为主入口
来源：http://est.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://fnh.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nzy.hfpthk.cn

JS:   require.main === module
来源：http://unb.52xcode.cn

TS:   require.main === module
来源：http://ylv.yj20258888.top

Java: public static void main(String[] args)
来源：http://cvu.hesvh.cn

Go:   func main()
来源：http://sjy.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nyz.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://qce.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://zie.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://rza.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://pwj.hesvh.cn

JS:   process.platform;  process.version
来源：http://xhg.hywenlv.cn

TS:   process.platform;  process.version
来源：http://sxh.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://upv.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vza.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vgk.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eqk.ybcxt.top

================================================================================
来源：http://hbd.zhengqikj.top

N. 数据结构与算法
来源：http://pra.nanxinkj.top

================================================================================
来源：http://aaz.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://xlp.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://mzz.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dqu.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rkv.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkh.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://ftz.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://boo.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fnu.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://ara.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://yhd.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://euq.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dhh.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qig.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://smh.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eth.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://toz.zdqjudy.top

Ruby: arr.sort
来源：http://gft.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oes.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://zwd.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lti.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://bqp.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkt.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fjm.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oep.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uxo.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://spb.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://vrk.iojbl.cn

[N04] 斐波那契数列
来源：http://mea.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://glv.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://brj.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryq.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stk.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hkm.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://egh.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jbc.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gve.epnwcf.com

[N05] 最大公约数
来源：http://hsz.uphjek.com

Py:   math.gcd(a, b)
来源：http://jrk.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ftj.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gke.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mcb.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://doj.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fnh.ppjwa.cn

Ruby: a.gcd(b)
来源：http://zvu.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjv.chenzaomai.com

[N06] 判断回文字符串
来源：http://eox.jqgfzy.top

Py:   s == s[::-1]
来源：http://mha.yj202588.top

PHP:  $s === strrev($s);
来源：http://vnm.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://fgh.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://ysf.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dbj.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://zhm.fehbvm.com

Ruby: s == s.reverse
来源：http://hwm.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ffm.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://qpp.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nzr.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://djm.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wfz.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://cem.fzhhl.top

Java: // 手写 HashMap
来源：http://zcb.ivvv.top

Go:   // 手写 map[int]int
来源：http://pgt.316326.xyz

Ruby: // 手写 Hash
来源：http://gjx.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://atb.yangfankeji.com

[N08] 生成全排列
来源：http://qdu.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://ilh.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://cem.cheryme.top

JS:   // 手写回溯递归
来源：http://wgh.andypj.xyz

TS:   // 手写回溯递归
来源：http://rtg.dashuyun.cn

Java: // 手写回溯递归
来源：http://oif.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://pbe.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://fpe.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://txi.hongshengwenyu.top

[N09] 栈与队列
来源：http://yqb.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tfq.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tln.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qrj.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omw.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fnw.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dtj.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://emn.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sek.gzhubu.top

[N10] 链表节点定义
来源：http://dks.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kej.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yat.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://twc.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmk.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://rlu.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cdj.fengsongda.top


<!-- 参考信息 -->