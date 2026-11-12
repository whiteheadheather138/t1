代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cck.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fnb.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mou.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lho.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tge.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bax.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eix.gotoacloud.top

[K05] 深拷贝对象
来源：http://drb.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://fym.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://fte.sufxvd.cn

JS:   structuredClone(obj)
来源：http://coy.epnwcf.com

TS:   structuredClone(obj)
来源：http://hdn.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zmi.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qgr.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://spl.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xcp.xziqi.cn

[K06] 解析 URL 查询串
来源：http://hmd.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ivp.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eql.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkr.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://buh.ydjk.org.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://osn.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dxk.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vml.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jwi.pengpengdd.cyou

[K07] 进制转换
来源：http://ueo.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://orx.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mlo.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://geo.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qkb.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ayq.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eww.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nml.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smi.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://cvb.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://jlq.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://chs.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://vpk.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://jej.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ong.uphjek.com

Go:   encoding/gob
来源：http://kwn.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://ncr.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dum.jlsjyb.cn

================================================================================
来源：http://rjn.bjfxy.top

L. 网络请求
来源：http://jis.yuxming.cn

================================================================================
来源：http://lxy.gogol.net.cn

[L01] 发送 GET 请求
来源：http://hhg.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jgg.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bgh.yanxiufei.cn

JS:   await fetch(url)
来源：http://ojo.pengpengdd.cyou

TS:   await fetch(url)
来源：http://bbi.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qqb.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://jdm.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zwj.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bll.fzhhl.top

[L02] 发送 POST JSON
来源：http://ent.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jrd.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cte.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdk.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myl.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pyn.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oes.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vex.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lpg.jqgfzy.top

[L03] 设置自定义请求头
来源：http://nid.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kmn.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xea.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gcn.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://esd.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hcu.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zgr.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fax.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zrp.guannengcc.top

[L04] 设置超时
来源：http://tuz.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://vcf.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mbj.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cxz.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gsz.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ddb.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pso.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jxu.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpc.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://nvm.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lvs.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbp.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zwd.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://thf.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cgj.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gos.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vdi.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://imb.pycfn.com

[L06] 解析响应为 JSON
来源：http://ktb.smart0.xyz

Py:   resp.json()
来源：http://qxx.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://frl.hcnkem.com

JS:   await resp.json()
来源：http://bbi.gogol.net.cn

TS:   await resp.json()
来源：http://oxz.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fbn.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tuh.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://nog.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://caw.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://lsg.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://igl.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pgz.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://tdm.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://jlg.nanxuanxn.top

Java: resp.statusCode()
来源：http://ckf.zhijiandao.cn

Go:   resp.StatusCode
来源：http://gwa.dianchejie.cn

Ruby: resp.code.to_i
来源：http://ppv.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://aku.wangdashe.top

[L08] 并发请求多个地址
来源：http://xca.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vgw.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://awh.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yge.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihn.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xoj.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rnz.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zdb.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mlm.yvedp.cn

================================================================================
来源：http://hob.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://ldj.bbcook.cn

================================================================================
来源：http://rzd.jlsjyb.cn

[M01] 读取命令行参数
来源：http://ajg.cheryme.top

Py:   sys.argv[1:]
来源：http://juv.hammf.cn

PHP:  $argv;  $argc;
来源：http://fww.yj202588.top

JS:   process.argv.slice(2)
来源：http://cjg.bjfxy.top

TS:   process.argv.slice(2)
来源：http://ipk.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://kgl.sjlbkw.cn

Go:   os.Args[1:]
来源：http://pqx.jianghu66.top

Ruby: ARGV
来源：http://gii.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://mxj.fzhhl.top

[M02] 读取环境变量
来源：http://oav.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://dgj.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jya.yanxiufei.cn

JS:   process.env.HOME
来源：http://myb.aizwys.cn

TS:   process.env.HOME
来源：http://mip.316326.xyz

Java: System.getenv("HOME")
来源：http://iid.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qek.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://dbq.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ioi.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://jbl.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ive.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pry.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jpe.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ovk.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdu.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rlo.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://xwo.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://uso.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://uav.gaohongyu789.top

Py:   os.getcwd()
来源：http://zmb.dianchejie.cn

PHP:  getcwd();
来源：http://wiq.iojbl.cn

JS:   process.cwd()
来源：http://yfb.guowangkeji.top

TS:   process.cwd()
来源：http://ndv.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://jji.sjlbkw.cn

Go:   os.Getwd()
来源：http://juq.yvedp.cn

Ruby: Dir.pwd
来源：http://ylp.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://agf.nanxuanxn.top

[M05] 设置退出码
来源：http://gmj.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://rcp.havefunace.top

PHP:  exit(1);
来源：http://jjk.jinqigufen.top

JS:   process.exit(1)
来源：http://itl.yongpay.top

TS:   process.exit(1)
来源：http://coj.cqqwz.cn

Java: System.exit(1)
来源：http://noq.birdmap.top

Go:   os.Exit(1)
来源：http://tvh.ctjpmb.com

Ruby: exit 1
来源：http://ybx.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://trg.0kj1m.cn

[M06] 向标准错误输出
来源：http://bgd.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://nzd.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://swb.jyoumei.cn

JS:   console.error("err")
来源：http://gmr.nwbrower.top

TS:   console.error("err")
来源：http://hrm.snrcjt.cn

Java: System.err.println("err")
来源：http://slh.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sxi.ybcxt.top

Ruby: warn "err"
来源：http://yxe.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://fsv.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://jga.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://yyv.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xjw.havefunace.top

JS:   require.main === module
来源：http://nlh.havefunace.top

TS:   require.main === module
来源：http://yfs.yangfankeji.com

Java: public static void main(String[] args)
来源：http://zph.jlsjyb.cn

Go:   func main()
来源：http://rpx.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://irn.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://orx.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://zae.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://dcg.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://mge.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://ive.ehwqpu.com

TS:   process.platform;  process.version
来源：http://fce.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fqj.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kst.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vit.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hme.tian-w.cn

================================================================================
来源：http://cff.bbcook.cn

N. 数据结构与算法
来源：http://ixo.fengsongda.top

================================================================================
来源：http://psq.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://vsd.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://akw.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lgm.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pot.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://spt.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://vvy.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://sxj.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://usg.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://djf.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://ytv.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://gge.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://muw.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vbj.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yud.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbq.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://czw.zdqjudy.top

Ruby: arr.sort
来源：http://beb.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wfx.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://rzr.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cpp.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://wen.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckm.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abq.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jff.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://shm.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://srr.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://zsd.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://rpx.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://owt.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uts.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oro.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gly.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ulw.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jsf.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bnv.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qxz.wangshuangyany.cn

[N05] 最大公约数
来源：http://dqn.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://slo.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uog.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eal.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hcu.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://thk.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gcq.gzhubu.top

Ruby: a.gcd(b)
来源：http://ehw.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nab.tarul.cn

[N06] 判断回文字符串
来源：http://lrt.52xcode.cn

Py:   s == s[::-1]
来源：http://zqm.iojbl.cn

PHP:  $s === strrev($s);
来源：http://fth.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://iwb.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://scv.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syx.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://lar.nwbrower.top

Ruby: s == s.reverse
来源：http://ioy.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sgt.sweek.top

[N07] 两数之和（返回下标）
来源：http://jgq.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hri.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fcj.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://utp.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://vuf.ctjpmb.com

Java: // 手写 HashMap
来源：http://uqb.hcnkem.com

Go:   // 手写 map[int]int
来源：http://iub.aibaodan.cn

Ruby: // 手写 Hash
来源：http://dwc.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://qvr.andypj.xyz

[N08] 生成全排列
来源：http://msc.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://vof.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://tto.yuxming.cn

JS:   // 手写回溯递归
来源：http://mwd.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://iol.gotoacloud.top

Java: // 手写回溯递归
来源：http://uds.pycfn.com

Go:   // 手写回溯递归
来源：http://tdz.cheryme.top

Ruby: arr.permutation.to_a
来源：http://kad.gzhubu.top

C#:   // 手写回溯递归
来源：http://xun.chenzaomai.com

[N09] 栈与队列
来源：http://vrv.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dgu.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://anw.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ibz.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpl.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mta.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rgx.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qcz.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xkd.ybcxt.top

[N10] 链表节点定义
来源：http://hlj.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fol.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://exz.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mvc.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fht.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://xyp.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cqd.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cpg.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dbj.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://wyg.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uyt.yangfankeji.com

PHP:  // 手写递归函数
来源：http://gyx.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovf.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fab.havefunace.top

Java: // 手写递归
来源：http://cbs.zhoulong.xyz

Go:   // 手写递归
来源：http://gzm.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hkt.cucudq.cn

C#:   // 手写递归
来源：http://rgn.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ffb.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ysx.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nha.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttq.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nof.fehbvm.com


<!-- 参考信息 -->