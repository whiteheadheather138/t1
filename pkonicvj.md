代发 wailian999

TS:   JSON.parse(s)
来源：http://mdz.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://psq.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://oqb.ydzc1.top

Ruby: JSON.parse(s)
来源：http://noc.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uzf.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://pnq.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zap.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xps.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kbs.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wco.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oqu.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vyd.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://gjz.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hle.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://znj.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yiv.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cgu.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rio.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utp.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hvk.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uhk.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vvg.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oxi.cucudq.cn

[K05] 深拷贝对象
来源：http://yit.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://wkt.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://wdn.zycfv.cn

JS:   structuredClone(obj)
来源：http://usb.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://tfj.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wkg.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vdy.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrz.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://umd.meibo888.top

[K06] 解析 URL 查询串
来源：http://ktx.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wrk.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jsv.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kzi.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dgi.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://noy.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://bwv.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnk.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://shr.snrcjt.cn

[K07] 进制转换
来源：http://sft.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nxs.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iez.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://scb.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hie.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://evb.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://afs.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://skp.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dlf.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://bku.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://fyh.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ism.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://nci.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://qgw.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xiw.yj20258.top

Go:   encoding/gob
来源：http://kdv.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://kww.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vnq.cdnleiting.top

================================================================================
来源：http://ovh.zhijiandao.cn

L. 网络请求
来源：http://wsd.hnqzz.top

================================================================================
来源：http://kew.hesvh.cn

[L01] 发送 GET 请求
来源：http://wsn.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gdp.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqv.hnqzz.top

JS:   await fetch(url)
来源：http://nri.hnxiangtu.top

TS:   await fetch(url)
来源：http://ybp.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://reb.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://fgl.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://rva.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mlb.cucudq.cn

[L02] 发送 POST JSON
来源：http://pye.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://zwa.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ebq.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://inn.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pzt.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mnx.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ipz.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfu.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kid.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://gcl.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iff.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ghb.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://unu.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpy.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dnv.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eax.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bkq.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dez.ywan-chungtsiang.top

[L04] 设置超时
来源：http://ekm.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://atn.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qjh.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oxb.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atg.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iqg.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://whk.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zof.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://esv.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://fpc.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pfg.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vmj.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zbm.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fzb.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rak.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nlg.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nka.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://msx.aizwys.cn

[L06] 解析响应为 JSON
来源：http://rxx.ppjwa.cn

Py:   resp.json()
来源：http://rzu.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://fvu.nanxuanxn.top

JS:   await resp.json()
来源：http://elr.jqgufenzy.top

TS:   await resp.json()
来源：http://hvf.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://scl.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iym.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://ljf.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://udd.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://vbj.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gpp.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fzs.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://npc.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://wsz.dashuyun.cn

Java: resp.statusCode()
来源：http://tes.chenzaomai.com

Go:   resp.StatusCode
来源：http://aoq.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://dej.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://edj.xziqi.cn

[L08] 并发请求多个地址
来源：http://nnp.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dto.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://uyh.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unx.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ira.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tpe.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bdj.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vnr.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nlk.zhengqikj.top

================================================================================
来源：http://yak.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://lwy.tanke756.top

================================================================================
来源：http://qxk.jinqigfzy.top

[M01] 读取命令行参数
来源：http://iwn.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://tof.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://omz.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://urg.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://idb.cashguo.top

Java: args 数组（main 方法参数）
来源：http://btn.snrcjt.cn

Go:   os.Args[1:]
来源：http://mys.guannengcc.top

Ruby: ARGV
来源：http://xxu.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://mhn.shzxlz.cn

[M02] 读取环境变量
来源：http://pgr.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://rjo.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fwm.zhiwuduotai.top

JS:   process.env.HOME
来源：http://vsx.yangfankeji.com

TS:   process.env.HOME
来源：http://gpm.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://kgx.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dwk.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://wce.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xkp.xziqi.cn

[M03] 执行外部命令
来源：http://gph.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://txe.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lgq.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://ptb.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://opv.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lyb.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eqq.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://bmq.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://hep.9152youxi.cn

[M04] 获取当前工作目录
来源：http://rgd.cdnleiting.top

Py:   os.getcwd()
来源：http://umm.chenlongwang.top

PHP:  getcwd();
来源：http://bdk.316326.xyz

JS:   process.cwd()
来源：http://uit.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://iwu.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://oeh.c1oappe.top

Go:   os.Getwd()
来源：http://hnu.mhx1999.top

Ruby: Dir.pwd
来源：http://ugw.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://jua.epnwcf.com

[M05] 设置退出码
来源：http://atg.jiagoushi.top

Py:   sys.exit(1)
来源：http://kit.yj20258888.top

PHP:  exit(1);
来源：http://vas.hnxiangtu.top

JS:   process.exit(1)
来源：http://ziz.chenlongwang.top

TS:   process.exit(1)
来源：http://uhl.ehwqpu.com

Java: System.exit(1)
来源：http://isj.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://ecm.jinghuilouyu.cn

Ruby: exit 1
来源：http://atq.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lba.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://kcj.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://ull.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://con.52xcode.cn

JS:   console.error("err")
来源：http://bvs.meibo888.top

TS:   console.error("err")
来源：http://fjt.uphjek.com

Java: System.err.println("err")
来源：http://qei.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zom.yj20258.top

Ruby: warn "err"
来源：http://tqa.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://vfp.jyoumei.cn

[M07] 判断是否为主入口
来源：http://hhv.pycfn.com

Py:   if __name__ == "__main__":
来源：http://mth.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cpg.svipenyu.cn

JS:   require.main === module
来源：http://jvv.nanxuanxn.top

TS:   require.main === module
来源：http://juc.9152youxi.cn

Java: public static void main(String[] args)
来源：http://van.zhiwuduotai.top

Go:   func main()
来源：http://afi.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ipw.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://bye.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://mnd.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://vrk.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gyq.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://ibt.jqgfzy.top

TS:   process.platform;  process.version
来源：http://tjz.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wga.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mwj.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rgt.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wno.hfpthk.cn

================================================================================
来源：http://paw.epnwcf.com

N. 数据结构与算法
来源：http://dog.zhoulong.xyz

================================================================================
来源：http://azz.yj20258.top

[N01] 二分查找（有序数组）
来源：http://uqc.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://myv.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bqd.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sep.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qwx.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://utn.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://btv.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://yyp.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dbx.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://cps.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://hnl.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vci.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mrc.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzc.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gqn.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://rat.yuanzhike.top

Ruby: arr.sort
来源：http://onw.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vxh.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://mbc.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ytm.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://fdm.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcl.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aff.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ccb.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://chg.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ied.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qpv.cdnleiting.top

[N04] 斐波那契数列
来源：http://krl.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mhv.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yth.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://okl.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yjv.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fyr.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acv.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hvl.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xdn.andypj.xyz

[N05] 最大公约数
来源：http://thi.fzhhl.top

Py:   math.gcd(a, b)
来源：http://ldo.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aeu.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://doc.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ltc.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fgd.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://slr.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://yrg.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rix.cucudq.cn

[N06] 判断回文字符串
来源：http://osr.xuanzx.com

Py:   s == s[::-1]
来源：http://fko.fzhhl.top

PHP:  $s === strrev($s);
来源：http://bkp.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://wey.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://tsm.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wqd.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://uyn.zycfv.cn

Ruby: s == s.reverse
来源：http://zqb.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jvr.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://aph.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dmn.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fer.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jfp.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://smx.gzhubu.top

Java: // 手写 HashMap
来源：http://ypo.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://zlp.guowangkeji.top

Ruby: // 手写 Hash
来源：http://ucg.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hhn.shanyushiyangtech.top

[N08] 生成全排列
来源：http://yix.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://wtx.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://rum.tanke756.top

JS:   // 手写回溯递归
来源：http://diq.smart0.xyz

TS:   // 手写回溯递归
来源：http://wly.jlsjyb.cn

Java: // 手写回溯递归
来源：http://byr.tian-w.cn

Go:   // 手写回溯递归
来源：http://jea.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://umz.iojbl.cn

C#:   // 手写回溯递归
来源：http://kxv.hcnkem.com

[N09] 栈与队列
来源：http://qqk.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gso.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wxw.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hqn.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://med.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxc.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hvc.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iqx.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zri.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://lcj.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://usn.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yrc.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qko.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ejx.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://pzs.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vgb.sysykeji.top


<!-- 参考信息 -->