代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://bqd.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bih.meibo888.top

[K04] 读取 JSON 文件
来源：http://xqb.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mcb.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rut.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bkl.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gim.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vep.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lek.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vsq.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://idc.yj20258.top

[K05] 深拷贝对象
来源：http://ghv.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://wom.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://foj.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://wmp.ctjpmb.com

TS:   structuredClone(obj)
来源：http://iec.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ffd.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxr.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hoe.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qdr.sweek.top

[K06] 解析 URL 查询串
来源：http://ecx.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yom.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://daj.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxf.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://acz.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zjs.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iuz.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnd.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ufp.iojbl.cn

[K07] 进制转换
来源：http://phy.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tmo.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ffb.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ajc.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tzo.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rmv.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cjb.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rzr.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://coi.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://vbw.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://ktl.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yss.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://ntf.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://qnr.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zvc.aizwys.cn

Go:   encoding/gob
来源：http://bbl.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://xim.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jyk.52xcode.cn

================================================================================
来源：http://rwb.birdmap.top

L. 网络请求
来源：http://aos.shangyingyoupin.top

================================================================================
来源：http://zzd.ydzc1.top

[L01] 发送 GET 请求
来源：http://qid.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pwh.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://phk.zhengqikj.top

JS:   await fetch(url)
来源：http://wzp.sysykeji.top

TS:   await fetch(url)
来源：http://wtt.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hcb.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://ljj.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ufc.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fzz.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://nzz.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://czs.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aog.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvo.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uey.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tch.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vjj.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://umh.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hda.jinqigufen.top

[L03] 设置自定义请求头
来源：http://vho.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tnv.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://azw.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kso.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvz.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uys.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fbe.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ydk.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://win.zdqjudy.top

[L04] 设置超时
来源：http://hfv.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://skq.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lhc.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gag.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xpk.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dnj.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vcc.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ymt.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://frr.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://vxx.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ldo.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aod.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pde.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wpg.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yjv.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bjj.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hrw.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dxc.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://klo.jqgfzy.top

Py:   resp.json()
来源：http://oue.yj20258888.top

PHP:  json_decode($body, true);
来源：http://cvx.jiagoushi.top

JS:   await resp.json()
来源：http://rhb.zhixingplan.top

TS:   await resp.json()
来源：http://ddb.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpf.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://utp.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://hvs.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wxa.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://xkq.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://weq.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aqo.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://yvj.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://cwv.chenjidiqi.icu

Java: resp.statusCode()
来源：http://gfw.dashuyun.cn

Go:   resp.StatusCode
来源：http://fmo.dianchejie.cn

Ruby: resp.code.to_i
来源：http://jhq.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://cfi.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://sdd.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wgy.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://rxc.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zyv.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zrj.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yvm.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mjn.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvn.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://shu.hammf.cn

================================================================================
来源：http://eua.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://uez.yj202588.top

================================================================================
来源：http://vuv.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://vbf.pycfn.com

Py:   sys.argv[1:]
来源：http://pyt.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://aoi.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://xiu.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://gnb.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://ket.hammf.cn

Go:   os.Args[1:]
来源：http://edj.fktsv.cn

Ruby: ARGV
来源：http://tmi.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://hfw.cheryme.top

[M02] 读取环境变量
来源：http://bgh.316326.xyz

Py:   os.environ.get("HOME")
来源：http://kdf.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oft.jianghu66.top

JS:   process.env.HOME
来源：http://cok.hongshengwenyu.top

TS:   process.env.HOME
来源：http://gji.xziqi.cn

Java: System.getenv("HOME")
来源：http://vma.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ynm.sweek.top

Ruby: ENV["HOME"]
来源：http://zgr.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dbg.uphjek.com

[M03] 执行外部命令
来源：http://lff.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xal.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cuj.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wil.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gcr.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dba.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fgn.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://vri.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://ati.nanxinkj.top

[M04] 获取当前工作目录
来源：http://qxr.cashguo.top

Py:   os.getcwd()
来源：http://wlw.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://wtw.xziqi.cn

JS:   process.cwd()
来源：http://ahh.hnqzz.top

TS:   process.cwd()
来源：http://gpj.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://gks.fzhhl.top

Go:   os.Getwd()
来源：http://rsc.nanxuanxn.top

Ruby: Dir.pwd
来源：http://tvo.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://gor.iojbl.cn

[M05] 设置退出码
来源：http://mhi.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://odj.svipenyu.cn

PHP:  exit(1);
来源：http://bei.fengsongda.top

JS:   process.exit(1)
来源：http://mfp.gogol.net.cn

TS:   process.exit(1)
来源：http://boo.wangshuangyany.cn

Java: System.exit(1)
来源：http://hfj.sxryk.cn

Go:   os.Exit(1)
来源：http://wls.guowangkeji.top

Ruby: exit 1
来源：http://bol.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xtf.vehdjk.com

[M06] 向标准错误输出
来源：http://yrv.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://kjb.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nyv.gotoacloud.top

JS:   console.error("err")
来源：http://bkd.tian-w.cn

TS:   console.error("err")
来源：http://ite.smart0.xyz

Java: System.err.println("err")
来源：http://ljc.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uec.ivvv.top

Ruby: warn "err"
来源：http://wrs.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://ope.chenlongwang.top

[M07] 判断是否为主入口
来源：http://ppa.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://pip.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsj.yonumen.top

JS:   require.main === module
来源：http://ffl.yuxming.cn

TS:   require.main === module
来源：http://haa.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://qyn.52xcode.cn

Go:   func main()
来源：http://cty.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sxh.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://bjv.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://xwq.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://xja.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://uyp.hfpthk.cn

JS:   process.platform;  process.version
来源：http://fsq.yangfankeji.com

TS:   process.platform;  process.version
来源：http://wit.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gur.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lfb.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://axz.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jmt.zycfv.cn

================================================================================
来源：http://eik.sweek.top

N. 数据结构与算法
来源：http://ydf.yuxming.cn

================================================================================
来源：http://wme.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://eyu.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://fzu.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ibf.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fez.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qhf.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://rhj.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://awa.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://svl.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xuz.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://ygc.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://qog.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bbc.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://seq.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zkz.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jdz.316326.xyz

Go:   slices.Sort(arr)
来源：http://mmg.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://tsu.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybl.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://cxv.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://amk.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://tok.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gzf.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dvx.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://itg.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hxb.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zwx.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yrw.havefunace.top

[N04] 斐波那契数列
来源：http://fqq.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vil.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mnn.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fjr.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lob.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bgu.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ksc.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rca.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cql.svipenyu.cn

[N05] 最大公约数
来源：http://liw.sxryk.cn

Py:   math.gcd(a, b)
来源：http://zwj.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zak.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mrg.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lfk.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cib.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfv.zdqjudy.top

Ruby: a.gcd(b)
来源：http://bsh.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tbx.cucudq.cn

[N06] 判断回文字符串
来源：http://htx.jianghu66.top

Py:   s == s[::-1]
来源：http://dyl.tarul.cn

PHP:  $s === strrev($s);
来源：http://tyj.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://usx.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://sze.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tgx.52xcode.cn

Go:   // 双指针从两端比较
来源：http://spv.fehbvm.com

Ruby: s == s.reverse
来源：http://cxb.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ovo.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://fcv.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zzz.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sek.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xtb.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://auq.cqqwz.cn

Java: // 手写 HashMap
来源：http://dzr.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ivv.sufxvd.cn

Ruby: // 手写 Hash
来源：http://ggg.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://xwt.aizwys.cn

[N08] 生成全排列
来源：http://ccm.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://yok.cucudq.cn

PHP:  // 手写递归交换
来源：http://qod.gogol.net.cn

JS:   // 手写回溯递归
来源：http://lvr.havefunace.top

TS:   // 手写回溯递归
来源：http://onv.cheryme.top

Java: // 手写回溯递归
来源：http://xgs.zhixingplan.top

Go:   // 手写回溯递归
来源：http://jkg.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://wuw.snrcjt.cn

C#:   // 手写回溯递归
来源：http://brc.mhx1999.top

[N09] 栈与队列
来源：http://vjc.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zpw.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yhu.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yad.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://quy.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uwi.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cjz.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wbr.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnr.sufxvd.cn

[N10] 链表节点定义
来源：http://eoe.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kcx.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vap.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tig.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fqb.yj20258.top

Java: class Node { int v; Node next; }
来源：http://mkg.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://krm.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://icg.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wux.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://iab.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zeo.yfazqb.com

PHP:  // 手写递归函数
来源：http://jou.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cgb.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ruy.yuxming.cn

Java: // 手写递归
来源：http://cyn.cheryme.top

Go:   // 手写递归
来源：http://lyg.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://juj.c1oappe.top

C#:   // 手写递归
来源：http://hrh.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hdu.yongpay.top


<!-- 参考信息 -->