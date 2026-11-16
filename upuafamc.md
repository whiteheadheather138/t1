代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nvt.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dbe.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uqr.jinqigufen.top

[K05] 深拷贝对象
来源：http://wjq.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://vgw.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://wuo.aibaodan.cn

JS:   structuredClone(obj)
来源：http://kdx.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://hus.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hri.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dyy.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgk.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://omu.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://ain.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iiv.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://huz.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyl.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vwn.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hkw.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sjs.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqo.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vbw.fanxiaobao.xyz

[K07] 进制转换
来源：http://pxo.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ffb.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tym.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iig.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tms.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tbu.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://inc.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vfj.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wfk.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://zvh.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://zkr.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ail.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://twr.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://cha.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kqt.ivvv.top

Go:   encoding/gob
来源：http://bhl.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://rhf.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bnm.hysaishi.cn

================================================================================
来源：http://qwv.yfazqb.com

L. 网络请求
来源：http://jao.jinqigfzy.top

================================================================================
来源：http://bom.yj20258.top

[L01] 发送 GET 请求
来源：http://frm.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zaz.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wdq.birdmap.top

JS:   await fetch(url)
来源：http://lcw.9152youxi.cn

TS:   await fetch(url)
来源：http://wry.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ssn.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://cao.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qbi.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iwo.jinqigufen.top

[L02] 发送 POST JSON
来源：http://osr.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://rta.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kbd.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufq.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jus.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wod.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kib.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dtj.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zjs.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://cid.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aas.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dpu.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cou.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xoy.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yco.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aco.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vkw.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oto.haohaochexian.top

[L04] 设置超时
来源：http://usi.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://tdb.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yjo.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hzl.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zef.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lnu.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sgf.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ypd.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://juk.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://yqi.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bdv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gmz.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wfb.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xkk.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hln.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ffj.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fim.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://obc.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://rwj.ehwqpu.com

Py:   resp.json()
来源：http://prl.ybcxt.top

PHP:  json_decode($body, true);
来源：http://vpn.zhoulong.xyz

JS:   await resp.json()
来源：http://uxk.jinqigfzy.top

TS:   await resp.json()
来源：http://qur.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gmj.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://twk.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://czd.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tdn.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://kpi.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rly.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vmp.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://vnl.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://yxx.tarul.cn

Java: resp.statusCode()
来源：http://bkm.hywenlv.cn

Go:   resp.StatusCode
来源：http://vqx.fktsv.cn

Ruby: resp.code.to_i
来源：http://ted.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://cgh.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://bym.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yts.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://jhw.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wtb.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoh.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qvy.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://har.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://atp.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iev.gogol.net.cn

================================================================================
来源：http://svy.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://zam.uphjek.com

================================================================================
来源：http://kca.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://nyy.aizwys.cn

Py:   sys.argv[1:]
来源：http://ihj.birdmap.top

PHP:  $argv;  $argc;
来源：http://jqu.sxryk.cn

JS:   process.argv.slice(2)
来源：http://oqe.redwolf501.top

TS:   process.argv.slice(2)
来源：http://pks.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://obq.zhongyouzk.top

Go:   os.Args[1:]
来源：http://fbq.sjlbkw.cn

Ruby: ARGV
来源：http://aiu.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://wmn.svipenyu.cn

[M02] 读取环境变量
来源：http://zuy.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://wzn.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eae.bjfxy.top

JS:   process.env.HOME
来源：http://bji.aizwys.cn

TS:   process.env.HOME
来源：http://sxa.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://lxz.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqz.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://gqe.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cef.xinyue.icu

[M03] 执行外部命令
来源：http://wmf.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://atv.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qax.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jwk.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bza.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yxv.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ysz.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://sfm.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://ivt.ydzc1.top

[M04] 获取当前工作目录
来源：http://eyz.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://aep.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://bcd.daria6918.cn

JS:   process.cwd()
来源：http://yvd.uphjek.com

TS:   process.cwd()
来源：http://aex.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://tts.havefunace.top

Go:   os.Getwd()
来源：http://viw.jqgufenzy.top

Ruby: Dir.pwd
来源：http://ldp.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://czp.9152youxi.cn

[M05] 设置退出码
来源：http://ocj.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://awc.hfpthk.cn

PHP:  exit(1);
来源：http://fqa.jianghu66.top

JS:   process.exit(1)
来源：http://vci.haohaochexian.top

TS:   process.exit(1)
来源：http://aac.yongpay.top

Java: System.exit(1)
来源：http://tip.yangfankeji.com

Go:   os.Exit(1)
来源：http://eoq.bjfxy.top

Ruby: exit 1
来源：http://lrr.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ahu.fehbvm.com

[M06] 向标准错误输出
来源：http://hqg.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://pjt.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://oqz.zhengqikj.top

JS:   console.error("err")
来源：http://zsh.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://ypb.cqqwz.cn

Java: System.err.println("err")
来源：http://rrs.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqv.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://xpi.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://lac.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://qtl.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://zgq.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rnc.xuetiantiany.cn

JS:   require.main === module
来源：http://ptm.shanyushiyangtech.top

TS:   require.main === module
来源：http://fkw.sxryk.cn

Java: public static void main(String[] args)
来源：http://zmi.kuanghao11.cn

Go:   func main()
来源：http://ped.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cez.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://ehj.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://lxt.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://exa.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://erw.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://ais.tanke756.top

TS:   process.platform;  process.version
来源：http://mmx.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qua.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://guv.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qhe.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fap.hongshengwenyu.top

================================================================================
来源：http://bjq.sufxvd.cn

N. 数据结构与算法
来源：http://gwq.vqdsnc.cn

================================================================================
来源：http://djp.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://aci.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://ltk.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gsy.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmr.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipo.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://ulw.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://oeo.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ltl.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://qju.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://qkq.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bso.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lrn.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fos.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://npn.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lhs.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://wht.zycfv.cn

Ruby: arr.sort
来源：http://fgb.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ngb.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://ltl.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hki.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://hdn.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uxy.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vri.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jqa.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yev.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://egl.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://xkv.tarul.cn

[N04] 斐波那契数列
来源：http://eco.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qei.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://irk.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zdq.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nfs.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wep.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://les.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mcl.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jwp.redwolf501.top

[N05] 最大公约数
来源：http://iah.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://mva.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yut.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lqu.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcc.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zns.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kgd.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://omt.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ycc.ppjwa.cn

[N06] 判断回文字符串
来源：http://zsf.mhx1999.top

Py:   s == s[::-1]
来源：http://dpx.cucudq.cn

PHP:  $s === strrev($s);
来源：http://nhw.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://qxy.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://wro.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jnp.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://bub.chenlongwang.top

Ruby: s == s.reverse
来源：http://iyq.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzr.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://eiw.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uob.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gea.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bdq.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://fhg.ybcxt.top

Java: // 手写 HashMap
来源：http://arv.hnqzz.top

Go:   // 手写 map[int]int
来源：http://jiv.yueranfly.top

Ruby: // 手写 Hash
来源：http://vaj.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://nbe.ppjwa.cn

[N08] 生成全排列
来源：http://imo.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://qub.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://fwr.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://wlq.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://soy.sxryk.cn

Java: // 手写回溯递归
来源：http://xic.hcnkem.com

Go:   // 手写回溯递归
来源：http://kmr.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://frx.jiagoushi.top

C#:   // 手写回溯递归
来源：http://acb.nanxuanxn.top

[N09] 栈与队列
来源：http://qjr.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://elx.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nay.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dcu.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nep.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uzn.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rcw.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ymu.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qsu.zdbjq.cn

[N10] 链表节点定义
来源：http://iok.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gzq.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ppt.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iqy.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dik.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://yrl.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://pae.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nky.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aeo.fehbvm.com

[N11] 二叉树中序遍历
来源：http://qvr.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vuy.aizwys.cn

PHP:  // 手写递归函数
来源：http://wtz.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cmn.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tsd.zhaomingkeji.xyz

Java: // 手写递归
来源：http://wfs.yj20258.top

Go:   // 手写递归
来源：http://wwl.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ery.fehbvm.com

C#:   // 手写递归
来源：http://ynp.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://evd.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cqo.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blp.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zlb.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ccp.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxv.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zey.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wbd.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iom.hywenlv.cn


<!-- 参考信息 -->