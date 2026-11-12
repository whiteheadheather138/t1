代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gfe.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vzt.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://twh.yj20258.top

[K05] 深拷贝对象
来源：http://bkc.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://lmw.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://xpa.pycfn.com

JS:   structuredClone(obj)
来源：http://tho.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://czv.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ydl.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://udi.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://znm.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zxs.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://jit.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eal.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwn.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgb.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nec.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://krs.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qoe.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sfd.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yvx.nwbrower.top

[K07] 进制转换
来源：http://bwh.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fgh.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dmp.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ctk.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jol.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzy.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mye.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uvv.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iac.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://rrr.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://ynp.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lbu.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ctt.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://sfx.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mal.hongshengwenyu.top

Go:   encoding/gob
来源：http://gyj.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://wxg.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xgz.fktsv.cn

================================================================================
来源：http://krj.hnqzz.top

L. 网络请求
来源：http://iwq.sweek.top

================================================================================
来源：http://ayz.ivvv.top

[L01] 发送 GET 请求
来源：http://tmb.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xha.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rxz.zhongyouzk.top

JS:   await fetch(url)
来源：http://qxh.ctjpmb.com

TS:   await fetch(url)
来源：http://psk.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://unu.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://gct.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vwd.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sdo.guowangkeji.top

[L02] 发送 POST JSON
来源：http://hlg.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://blc.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rpf.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://omb.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffy.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://igo.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qbe.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dhb.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mfj.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://cpy.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gqf.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zmm.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tty.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://prn.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wqe.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lbq.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xuu.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wzm.yangfankeji.com

[L04] 设置超时
来源：http://zkq.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://zut.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://thh.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjp.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmv.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nkx.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vkx.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://buo.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dfl.shuidangran.top

[L05] 上传文件（multipart）
来源：http://kjp.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yvs.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uyd.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://obs.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bfi.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqc.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://thl.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nci.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jkt.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://iju.zhongyouzk.top

Py:   resp.json()
来源：http://pea.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://yxo.sufxvd.cn

JS:   await resp.json()
来源：http://vme.gogol.net.cn

TS:   await resp.json()
来源：http://jxb.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xxa.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ylq.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://plp.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ykc.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://kem.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jgv.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uae.yj20258.top

JS:   resp.ok;  resp.status
来源：http://hrv.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://bkp.fengsongda.top

Java: resp.statusCode()
来源：http://vpc.vqdsnc.cn

Go:   resp.StatusCode
来源：http://dei.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://oap.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://lyu.jiagoushi.top

[L08] 并发请求多个地址
来源：http://igx.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zpc.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://wvg.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxm.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gvh.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aih.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sej.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zig.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vgg.chenlongwang.top

================================================================================
来源：http://hoc.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://gei.zhongyouzk.top

================================================================================
来源：http://uzb.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://keu.cdnleiting.top

Py:   sys.argv[1:]
来源：http://fds.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://muo.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://ajl.meibo888.top

TS:   process.argv.slice(2)
来源：http://qba.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://tev.jqgfzy.top

Go:   os.Args[1:]
来源：http://spo.zhijiandao.cn

Ruby: ARGV
来源：http://cef.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://jqs.dashuyun.cn

[M02] 读取环境变量
来源：http://zpv.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://zbv.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://utr.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://dhu.jyoumei.cn

TS:   process.env.HOME
来源：http://xbl.jiagoushi.top

Java: System.getenv("HOME")
来源：http://cuc.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xbr.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://mbz.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gsf.sufxvd.cn

[M03] 执行外部命令
来源：http://hjz.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pqc.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tsa.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ewf.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sql.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mpq.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gcf.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mtl.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://hxs.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://rip.yueranfly.top

Py:   os.getcwd()
来源：http://ezp.uphjek.com

PHP:  getcwd();
来源：http://gjb.pengpengdd.cyou

JS:   process.cwd()
来源：http://mdi.zhiwuduotai.top

TS:   process.cwd()
来源：http://pqy.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://cdl.hesvh.cn

Go:   os.Getwd()
来源：http://dec.gaohongyu789.top

Ruby: Dir.pwd
来源：http://vli.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://yka.zycfv.cn

[M05] 设置退出码
来源：http://wcp.sjlbkw.cn

Py:   sys.exit(1)
来源：http://whz.yj20258.top

PHP:  exit(1);
来源：http://qld.nwbrower.top

JS:   process.exit(1)
来源：http://apn.cqqwz.cn

TS:   process.exit(1)
来源：http://uhr.gogol.net.cn

Java: System.exit(1)
来源：http://pos.tianlin.xyz

Go:   os.Exit(1)
来源：http://qes.vqdsnc.cn

Ruby: exit 1
来源：http://fkz.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ykm.sufxvd.cn

[M06] 向标准错误输出
来源：http://rva.hesvh.cn

Py:   print("err", file=sys.stderr)
来源：http://jhv.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qez.cdnleiting.top

JS:   console.error("err")
来源：http://rjj.52xcode.cn

TS:   console.error("err")
来源：http://qnn.gogol.net.cn

Java: System.err.println("err")
来源：http://wyb.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wrx.guannengcc.top

Ruby: warn "err"
来源：http://hcz.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://dda.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://qrb.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://oqx.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vve.xylfe.cn

JS:   require.main === module
来源：http://bit.shanyushiyangkeji.top

TS:   require.main === module
来源：http://rib.yonumen.top

Java: public static void main(String[] args)
来源：http://hfp.aibaodan.cn

Go:   func main()
来源：http://pcv.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://csa.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://pri.yongpay.top

[M08] 获取系统与运行时信息
来源：http://wrk.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://dfx.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://vsy.zhixingplan.top

JS:   process.platform;  process.version
来源：http://erk.cqqwz.cn

TS:   process.platform;  process.version
来源：http://nmh.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pnp.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tyl.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vhm.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsk.jinqigufen.top

================================================================================
来源：http://mmi.quarkkingdee.top

N. 数据结构与算法
来源：http://uik.cashguo.top

================================================================================
来源：http://ajl.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://jxc.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://tqx.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://srd.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xhd.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zbl.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uua.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://alr.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://okn.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://owa.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://bxu.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://tqr.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qdh.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ova.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://stb.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gra.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://hqw.jyoumei.cn

Ruby: arr.sort
来源：http://hbb.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tmv.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://yuv.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qnt.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://mip.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dsc.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://caz.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uvs.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zhb.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://txn.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://jyc.wangdashe.top

[N04] 斐波那契数列
来源：http://gwe.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iup.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ihy.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acq.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmj.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vqw.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ebm.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eti.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xkn.fengsongda.top

[N05] 最大公约数
来源：http://jdb.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://pyf.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://neu.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wkr.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ftv.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://opf.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxl.jinqigufen.top

Ruby: a.gcd(b)
来源：http://yvz.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dew.zhijiandao.cn

[N06] 判断回文字符串
来源：http://akr.bbcook.cn

Py:   s == s[::-1]
来源：http://cyv.yonumen.top

PHP:  $s === strrev($s);
来源：http://cqa.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://roq.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://usy.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nng.fktsv.cn

Go:   // 双指针从两端比较
来源：http://kuw.yj202588.top

Ruby: s == s.reverse
来源：http://qoq.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://quu.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://xuw.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hmp.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ydp.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://apl.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://tau.cqqwz.cn

Java: // 手写 HashMap
来源：http://afe.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://zmy.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://uum.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://hnd.shuidangran.top

[N08] 生成全排列
来源：http://hpj.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://ctr.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://ybv.fktsv.cn

JS:   // 手写回溯递归
来源：http://yur.pycfn.com

TS:   // 手写回溯递归
来源：http://msz.sysykeji.top

Java: // 手写回溯递归
来源：http://xdx.ctjpmb.com

Go:   // 手写回溯递归
来源：http://fsi.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://ekv.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://xzg.yueranfly.top

[N09] 栈与队列
来源：http://skq.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ufj.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hlz.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ulf.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hkx.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yxe.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sfg.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zif.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://for.cqqwz.cn

[N10] 链表节点定义
来源：http://hvw.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ksu.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gmj.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://igf.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qgd.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://yep.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dor.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mie.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://edk.jianghu66.top

[N11] 二叉树中序遍历
来源：http://qep.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ard.yuxming.cn

PHP:  // 手写递归函数
来源：http://vdr.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ecq.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nuq.zhixingplan.top

Java: // 手写递归
来源：http://tac.0kj1m.cn

Go:   // 手写递归
来源：http://mwn.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sin.fehbvm.com

C#:   // 手写递归
来源：http://msr.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kgc.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifq.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ujz.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://guf.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wln.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cop.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ngg.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aoz.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://srb.sxryk.cn


<!-- 参考信息 -->