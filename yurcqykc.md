代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qsj.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fsv.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gia.quarkkingdee.top

[K05] 深拷贝对象
来源：http://utw.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://qej.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://afj.sxryk.cn

JS:   structuredClone(obj)
来源：http://fkk.chenlongwang.top

TS:   structuredClone(obj)
来源：http://znf.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aju.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kke.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axq.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://raa.gzhubu.top

[K06] 解析 URL 查询串
来源：http://kbr.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uvf.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zrw.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytk.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uld.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zmu.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ohm.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zty.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xhq.fehbvm.com

[K07] 进制转换
来源：http://oyo.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cjf.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zzm.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fse.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vcx.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xna.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gbc.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hml.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qwd.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://wks.yonumen.top

Py:   pickle.dumps(obj)
来源：http://hrx.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vfh.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://tco.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://jux.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sfe.daria6918.cn

Go:   encoding/gob
来源：http://ezr.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://fxk.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kuw.sufxvd.cn

================================================================================
来源：http://kkb.gogol.net.cn

L. 网络请求
来源：http://awk.hcnkem.com

================================================================================
来源：http://sbr.fehbvm.com

[L01] 发送 GET 请求
来源：http://ngr.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rxs.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uvv.sxryk.cn

JS:   await fetch(url)
来源：http://irb.mhx1999.top

TS:   await fetch(url)
来源：http://zfy.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mat.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://fxg.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pvh.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sgm.bbcook.cn

[L02] 发送 POST JSON
来源：http://vyu.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yfj.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xow.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aul.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsu.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://asr.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zgk.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rop.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zaa.pycfn.com

[L03] 设置自定义请求头
来源：http://vnd.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udr.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pqo.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfe.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pss.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zji.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hjq.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yne.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yav.zhixingplan.top

[L04] 设置超时
来源：http://req.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://adr.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ija.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://emn.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://llh.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rdr.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yir.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ggg.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dhr.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://aie.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cpi.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvy.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jma.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xcp.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gir.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lth.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ukd.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fnn.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://aig.ydzc1.top

Py:   resp.json()
来源：http://grb.daria6918.cn

PHP:  json_decode($body, true);
来源：http://bao.guowangkeji.top

JS:   await resp.json()
来源：http://rlf.jinghuilouyu.cn

TS:   await resp.json()
来源：http://sdk.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lbj.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gxc.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://zji.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mrt.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://gcx.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gir.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lcn.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://iab.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://lko.bjfxy.top

Java: resp.statusCode()
来源：http://uzh.mhx1999.top

Go:   resp.StatusCode
来源：http://lmr.yj20258888.top

Ruby: resp.code.to_i
来源：http://dzd.tarul.cn

C#:   (int)resp.StatusCode
来源：http://cyu.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://gtq.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ouz.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://sve.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfn.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dym.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://opm.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tco.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bud.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://enz.jinqigufen.top

================================================================================
来源：http://mjh.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://hgw.sjlbkw.cn

================================================================================
来源：http://agu.9152youxi.cn

[M01] 读取命令行参数
来源：http://uza.hywenlv.cn

Py:   sys.argv[1:]
来源：http://ugi.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://uaw.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://uzo.gzhubu.top

TS:   process.argv.slice(2)
来源：http://pxe.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://lzw.tian-w.cn

Go:   os.Args[1:]
来源：http://zkg.yonumen.top

Ruby: ARGV
来源：http://yyl.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://mgo.hfpthk.cn

[M02] 读取环境变量
来源：http://kzv.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://ocx.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yks.dianchejie.cn

JS:   process.env.HOME
来源：http://npl.jyoumei.cn

TS:   process.env.HOME
来源：http://ssm.fktsv.cn

Java: System.getenv("HOME")
来源：http://cyd.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iii.fehbvm.com

Ruby: ENV["HOME"]
来源：http://kds.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fql.mhx1999.top

[M03] 执行外部命令
来源：http://qwl.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pyr.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oux.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zxx.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwe.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bjv.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vus.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://vqf.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://uds.jqgfzy.top

[M04] 获取当前工作目录
来源：http://kou.zhongyouzk.top

Py:   os.getcwd()
来源：http://dhi.redwolf501.top

PHP:  getcwd();
来源：http://kgy.uphjek.com

JS:   process.cwd()
来源：http://ntx.cdnleiting.top

TS:   process.cwd()
来源：http://myc.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://loh.nanxinkj.top

Go:   os.Getwd()
来源：http://jhd.ybcxt.top

Ruby: Dir.pwd
来源：http://zvv.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://irp.shanyushiyangtech.top

[M05] 设置退出码
来源：http://rsl.daria6918.cn

Py:   sys.exit(1)
来源：http://rrj.c1oappe.top

PHP:  exit(1);
来源：http://hpx.cucudq.cn

JS:   process.exit(1)
来源：http://ufz.jlsjyb.cn

TS:   process.exit(1)
来源：http://yxx.zhengqikj.top

Java: System.exit(1)
来源：http://rhc.sjlbkw.cn

Go:   os.Exit(1)
来源：http://ixy.tianlin.xyz

Ruby: exit 1
来源：http://vsa.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nli.yj20258888.top

[M06] 向标准错误输出
来源：http://occ.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://zhm.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zsf.havefunace.top

JS:   console.error("err")
来源：http://uov.zhongyouzk.top

TS:   console.error("err")
来源：http://gjr.daxiang520.top

Java: System.err.println("err")
来源：http://isx.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqu.kuanghao11.cn

Ruby: warn "err"
来源：http://jeu.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://owt.chenzaomai.com

[M07] 判断是否为主入口
来源：http://lec.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://uii.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://avd.svipenyu.cn

JS:   require.main === module
来源：http://qzq.ydzc1.top

TS:   require.main === module
来源：http://xtj.jyoumei.cn

Java: public static void main(String[] args)
来源：http://mgb.gaohongyu789.top

Go:   func main()
来源：http://wgl.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xiw.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://vfo.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://gbq.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://zzu.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://rso.chenlongwang.top

JS:   process.platform;  process.version
来源：http://vzh.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://ntm.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jad.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uph.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpy.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fka.yongpay.top

================================================================================
来源：http://qjt.pengpengdd.cyou

N. 数据结构与算法
来源：http://zok.ydzc1.top

================================================================================
来源：http://ecp.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://zpg.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://fbd.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrx.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alp.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywa.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://cjm.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://rzw.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gee.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://ixr.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://bzb.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://efd.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mye.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vtj.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jip.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sfr.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://qef.dianchejie.cn

Ruby: arr.sort
来源：http://tic.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ehh.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://sum.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yrs.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://abw.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dns.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scx.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gvr.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zec.wangdashe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xjb.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://jfy.zdbjq.cn

[N04] 斐波那契数列
来源：http://pag.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dsb.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wdy.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qci.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xoc.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://don.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lqq.bjfxy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fia.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqb.jiagoushi.top

[N05] 最大公约数
来源：http://tda.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://twj.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://czn.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgk.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pwg.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nde.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gjf.xziqi.cn

Ruby: a.gcd(b)
来源：http://brc.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pdm.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://gxa.sxryk.cn

Py:   s == s[::-1]
来源：http://adc.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://mcp.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://enc.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://byu.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jlq.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://swe.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://nak.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://meu.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://jqz.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ssq.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axk.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://res.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://vaj.yongpay.top

Java: // 手写 HashMap
来源：http://ojr.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://wta.ehwqpu.com

Ruby: // 手写 Hash
来源：http://rvt.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://bdq.haohaochexian.top

[N08] 生成全排列
来源：http://ygk.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://cmn.jianghu66.top

PHP:  // 手写递归交换
来源：http://qpf.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://sok.nwbrower.top

TS:   // 手写回溯递归
来源：http://fkh.vqdsnc.cn

Java: // 手写回溯递归
来源：http://pmd.meibo888.top

Go:   // 手写回溯递归
来源：http://mke.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://yyp.yuxming.cn

C#:   // 手写回溯递归
来源：http://pzw.hnxiangtu.top

[N09] 栈与队列
来源：http://jpl.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ftt.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sne.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iqb.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fch.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iof.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fuj.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wfb.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fjg.jqgfzy.top

[N10] 链表节点定义
来源：http://lzp.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fwr.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sxj.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hew.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qnw.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://btc.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://faf.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qve.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://akw.52xcode.cn

[N11] 二叉树中序遍历
来源：http://kez.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://geu.zhixingplan.top

PHP:  // 手写递归函数
来源：http://zey.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nec.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jyc.316326.xyz

Java: // 手写递归
来源：http://kdm.chenzaomai.com

Go:   // 手写递归
来源：http://tmz.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fsq.sweek.top

C#:   // 手写递归
来源：http://bvb.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dfn.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cgr.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://npy.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lev.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bdv.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbk.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://isl.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://alt.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rta.ywan-chungtsiang.top


<!-- 参考信息 -->