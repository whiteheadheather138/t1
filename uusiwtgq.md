代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://azl.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://ejj.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://plh.wangdashe.top

TS:   structuredClone(obj)
来源：http://ptr.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ufk.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fla.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xcf.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jbz.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://uka.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vmg.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bws.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcb.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eyq.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zvd.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cqz.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xos.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bky.birdmap.top

[K07] 进制转换
来源：http://cdl.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dgl.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zsz.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://biq.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gvx.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://asz.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zuf.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gys.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://paq.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://hbk.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://xjj.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ubm.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://hzj.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://hvh.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ovg.hywenlv.cn

Go:   encoding/gob
来源：http://cyf.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://xjf.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wsd.ehwqpu.com

================================================================================
来源：http://hks.redwolf501.top

L. 网络请求
来源：http://oxg.pycfn.com

================================================================================
来源：http://kkt.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://sds.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://key.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ihb.jiagoushi.top

JS:   await fetch(url)
来源：http://lxn.gotoacloud.top

TS:   await fetch(url)
来源：http://sym.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ged.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://tgj.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nye.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://upm.ydzc1.top

[L02] 发送 POST JSON
来源：http://vxf.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://enn.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ejr.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbc.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vcf.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://axn.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wyn.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wvz.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uwr.yj20258.top

[L03] 设置自定义请求头
来源：http://ldf.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cgl.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qme.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwl.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jve.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://evz.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ixl.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfm.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wdj.yuanzhike.top

[L04] 设置超时
来源：http://uko.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://yud.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bfd.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzk.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jih.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fud.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cuy.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://duo.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tyy.sweek.top

[L05] 上传文件（multipart）
来源：http://uzg.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://acq.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gza.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bmu.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xcj.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ebv.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ikf.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://een.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ykm.fehbvm.com

[L06] 解析响应为 JSON
来源：http://axo.sweek.top

Py:   resp.json()
来源：http://qnf.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://grx.gzhubu.top

JS:   await resp.json()
来源：http://pfg.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://zvp.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ktj.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fya.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://zec.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnw.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://sws.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://grm.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tob.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://lhz.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://azy.wangdashe.top

Java: resp.statusCode()
来源：http://zqu.aibaodan.cn

Go:   resp.StatusCode
来源：http://wrn.yuxming.cn

Ruby: resp.code.to_i
来源：http://gjy.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://kpe.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://hbu.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dyw.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://kah.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pnk.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ebi.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lzj.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mwo.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mhj.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mhn.9152youxi.cn

================================================================================
来源：http://jgo.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://bnf.kuanghao11.cn

================================================================================
来源：http://gng.pycfn.com

[M01] 读取命令行参数
来源：http://zux.0kj1m.cn

Py:   sys.argv[1:]
来源：http://wwk.yj202588.top

PHP:  $argv;  $argc;
来源：http://yyx.wangdashe.top

JS:   process.argv.slice(2)
来源：http://pat.cheryme.top

TS:   process.argv.slice(2)
来源：http://kxs.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://aqp.cdnleiting.top

Go:   os.Args[1:]
来源：http://sxb.sweek.top

Ruby: ARGV
来源：http://gom.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://kkc.fehbvm.com

[M02] 读取环境变量
来源：http://xqr.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://riv.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ncu.hnqzz.top

JS:   process.env.HOME
来源：http://zrk.nanxuanxn.top

TS:   process.env.HOME
来源：http://czb.smart0.xyz

Java: System.getenv("HOME")
来源：http://eus.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbj.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://pgw.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ooo.cdnleiting.top

[M03] 执行外部命令
来源：http://xsm.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ppb.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jwz.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ekr.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ghf.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jcf.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jjz.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://omf.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://qqf.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://iip.ydzc1.top

Py:   os.getcwd()
来源：http://qxm.ybcxt.top

PHP:  getcwd();
来源：http://ozc.jianghu66.top

JS:   process.cwd()
来源：http://fcs.andypj.xyz

TS:   process.cwd()
来源：http://dyx.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://dxy.zhixingplan.top

Go:   os.Getwd()
来源：http://gzf.gotoacloud.top

Ruby: Dir.pwd
来源：http://uic.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://qup.cqqwz.cn

[M05] 设置退出码
来源：http://qdb.bjfxy.top

Py:   sys.exit(1)
来源：http://azk.gogol.net.cn

PHP:  exit(1);
来源：http://vav.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://tcx.ydzc1.top

TS:   process.exit(1)
来源：http://ylf.svipenyu.cn

Java: System.exit(1)
来源：http://bgz.chenlongwang.top

Go:   os.Exit(1)
来源：http://rsz.zdbjq.cn

Ruby: exit 1
来源：http://srw.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fto.xinyue.icu

[M06] 向标准错误输出
来源：http://deh.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://guz.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rwb.316326.xyz

JS:   console.error("err")
来源：http://znq.sweek.top

TS:   console.error("err")
来源：http://eav.chenlongwang.top

Java: System.err.println("err")
来源：http://kdz.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bke.epnwcf.com

Ruby: warn "err"
来源：http://cxn.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://lga.zhixingplan.top

[M07] 判断是否为主入口
来源：http://fyp.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://hxs.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jrx.9152youxi.cn

JS:   require.main === module
来源：http://rus.zhengqikj.top

TS:   require.main === module
来源：http://cyd.tianlin.xyz

Java: public static void main(String[] args)
来源：http://zrk.yonumen.top

Go:   func main()
来源：http://ryu.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdz.fengsongda.top

C#:   static void Main(string[] args)
来源：http://iqr.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://ttw.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://zeh.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://psu.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://gtw.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://dzu.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://otq.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ckc.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzh.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vfq.yj20258.top

================================================================================
来源：http://pzp.pycfn.com

N. 数据结构与算法
来源：http://dhz.jqgufenzy.top

================================================================================
来源：http://gxi.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://lri.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://bzt.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://glv.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpa.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aig.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://bht.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://ign.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://nxy.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dof.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://syr.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://ydu.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ihk.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fph.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mty.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vxh.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://cdh.haohaochexian.top

Ruby: arr.sort
来源：http://imf.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xpg.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://lbp.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sdx.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://uxq.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aov.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sff.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kxz.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kop.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://npe.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ktb.jqgfzy.top

[N04] 斐波那契数列
来源：http://vev.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kbg.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xsi.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovb.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fit.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ulc.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xdc.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wna.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qmz.xuanzx.com

[N05] 最大公约数
来源：http://ree.pycfn.com

Py:   math.gcd(a, b)
来源：http://yyp.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fiz.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aqf.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpa.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nlj.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dmk.yj202588.top

Ruby: a.gcd(b)
来源：http://mlt.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sru.haohaochexian.top

[N06] 判断回文字符串
来源：http://vey.yj20258888.top

Py:   s == s[::-1]
来源：http://lsn.sxryk.cn

PHP:  $s === strrev($s);
来源：http://irw.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://spo.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://vxj.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mal.iojbl.cn

Go:   // 双指针从两端比较
来源：http://jzw.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://uwo.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://udf.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://fhh.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ayz.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lnc.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rfk.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://cdb.yanxiufei.cn

Java: // 手写 HashMap
来源：http://cio.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://aab.hammf.cn

Ruby: // 手写 Hash
来源：http://axb.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jgu.quarkkingdee.top

[N08] 生成全排列
来源：http://zyb.yj202588.top

Py:   itertools.permutations(arr)
来源：http://fqs.ybcxt.top

PHP:  // 手写递归交换
来源：http://obw.andypj.xyz

JS:   // 手写回溯递归
来源：http://dse.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://gqr.guowangkeji.top

Java: // 手写回溯递归
来源：http://ofn.yueranfly.top

Go:   // 手写回溯递归
来源：http://rlu.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://ncn.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://ope.mhx1999.top

[N09] 栈与队列
来源：http://mfy.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hsc.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bmv.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://atv.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hop.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzt.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewh.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ric.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lpv.hnqzz.top

[N10] 链表节点定义
来源：http://awl.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kjc.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cfr.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tzt.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bdo.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://uor.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://jja.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://neg.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://soh.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://mez.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gqf.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://yxz.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bsk.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fph.wangdashe.top

Java: // 手写递归
来源：http://loj.ivvv.top

Go:   // 手写递归
来源：http://jzx.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jii.fktsv.cn

C#:   // 手写递归
来源：http://esh.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qbe.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifd.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewx.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://crw.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgx.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qpn.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ivh.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pwp.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kos.yj20258888.top

================================================================================
来源：http://cbi.chenzaomai.com

O. 并发与异步
来源：http://ghk.shzxlz.cn

================================================================================
来源：http://auz.andypj.xyz

[O01] 启动一个线程
来源：http://jgr.shangyingyoupin.top


<!-- 参考信息 -->