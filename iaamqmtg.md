代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yvi.ivvv.top

[K07] 进制转换
来源：http://dyr.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://unk.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pvq.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pbx.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tpz.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gel.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://emr.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zed.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dmt.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://ijt.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://cdz.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ofj.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://gcq.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://ojq.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://npk.yonumen.top

Go:   encoding/gob
来源：http://pjz.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://rzo.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://itl.52xcode.cn

================================================================================
来源：http://gud.aizwys.cn

L. 网络请求
来源：http://txc.ydjk.org.cn

================================================================================
来源：http://fom.shuidangran.top

[L01] 发送 GET 请求
来源：http://xdq.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://irf.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pps.0kj1m.cn

JS:   await fetch(url)
来源：http://mog.quarkkingdee.top

TS:   await fetch(url)
来源：http://eyw.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eqe.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://dcn.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nch.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://twu.xuanzx.com

[L02] 发送 POST JSON
来源：http://mnj.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://uxz.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qcf.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlw.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ggi.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://syc.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ynd.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ial.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ndf.tianlin.xyz

[L03] 设置自定义请求头
来源：http://lmn.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ohq.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ajy.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evz.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qms.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hul.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sqx.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pph.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://klt.zdqjudy.top

[L04] 设置超时
来源：http://xrz.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://ogu.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qbj.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdt.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xga.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dzs.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqh.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xnb.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uzd.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://ire.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ihv.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://htj.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rjc.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kxl.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://acu.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sjh.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dgb.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uqm.ivvv.top

[L06] 解析响应为 JSON
来源：http://sfu.zhixingplan.top

Py:   resp.json()
来源：http://plr.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://jcu.cqqwz.cn

JS:   await resp.json()
来源：http://oxy.haohaochexian.top

TS:   await resp.json()
来源：http://ztq.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wrh.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rbb.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://twu.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://msh.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://wap.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mtm.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fra.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://ycf.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://baw.chenzaomai.com

Java: resp.statusCode()
来源：http://qre.quarkkingdee.top

Go:   resp.StatusCode
来源：http://opq.yfazqb.com

Ruby: resp.code.to_i
来源：http://dmh.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://kng.bbcook.cn

[L08] 并发请求多个地址
来源：http://kpj.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gmn.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://frg.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ect.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cer.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sfk.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vvy.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rrl.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tjb.zdbjq.cn

================================================================================
来源：http://tun.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://wan.yj20258888.top

================================================================================
来源：http://vxv.c1oappe.top

[M01] 读取命令行参数
来源：http://iwi.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://yuj.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://tig.ybcxt.top

JS:   process.argv.slice(2)
来源：http://uuc.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://ngm.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://gpj.jqgfzy.top

Go:   os.Args[1:]
来源：http://coi.zhiwuduotai.top

Ruby: ARGV
来源：http://rea.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://cjj.jinqigfzy.top

[M02] 读取环境变量
来源：http://tnf.havefunace.top

Py:   os.environ.get("HOME")
来源：http://vha.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wsq.zhoulong.xyz

JS:   process.env.HOME
来源：http://ula.birdmap.top

TS:   process.env.HOME
来源：http://ohk.hcnkem.com

Java: System.getenv("HOME")
来源：http://exw.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://myc.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://viw.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iol.jinqigufen.top

[M03] 执行外部命令
来源：http://wuu.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hlv.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gwl.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nnn.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ymt.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kne.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aoz.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://nuy.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://dax.jianghu66.top

[M04] 获取当前工作目录
来源：http://cvf.yonumen.top

Py:   os.getcwd()
来源：http://vga.hammf.cn

PHP:  getcwd();
来源：http://fwq.havefunace.top

JS:   process.cwd()
来源：http://tph.haohaochexian.top

TS:   process.cwd()
来源：http://lpe.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://jdk.hywenlv.cn

Go:   os.Getwd()
来源：http://krq.wangdashe.top

Ruby: Dir.pwd
来源：http://odp.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ehi.hammf.cn

[M05] 设置退出码
来源：http://vgf.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://ujb.nwbrower.top

PHP:  exit(1);
来源：http://zir.hnxiangtu.top

JS:   process.exit(1)
来源：http://tks.hesvh.cn

TS:   process.exit(1)
来源：http://lmg.xuanzx.com

Java: System.exit(1)
来源：http://efy.ydzc1.top

Go:   os.Exit(1)
来源：http://que.gzhubu.top

Ruby: exit 1
来源：http://nhc.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wgp.haohaochexian.top

[M06] 向标准错误输出
来源：http://ods.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://nwj.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pba.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://fiz.ydjk.org.cn

TS:   console.error("err")
来源：http://lhh.ctjpmb.com

Java: System.err.println("err")
来源：http://yyf.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qwd.kuanghao11.cn

Ruby: warn "err"
来源：http://xug.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://hsb.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://mhq.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://yjz.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rau.haohaochexian.top

JS:   require.main === module
来源：http://iuh.pengpengdd.cyou

TS:   require.main === module
来源：http://xqs.zycfv.cn

Java: public static void main(String[] args)
来源：http://zfb.cucudq.cn

Go:   func main()
来源：http://ess.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xya.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://rnb.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://rec.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://ivh.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://aow.xinyue.icu

JS:   process.platform;  process.version
来源：http://lqq.yj20258.top

TS:   process.platform;  process.version
来源：http://wlo.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brm.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nab.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://huc.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wxe.havefunace.top

================================================================================
来源：http://sqp.xziqi.cn

N. 数据结构与算法
来源：http://any.zhixingplan.top

================================================================================
来源：http://sgg.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://byp.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vcd.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tpc.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vko.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bwv.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://htv.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://naa.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mwn.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pak.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://nyb.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://zub.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bhf.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ayn.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xpa.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://scl.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://jqn.hfpthk.cn

Ruby: arr.sort
来源：http://wxa.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kim.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://dff.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jgm.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://dtf.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgg.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://snb.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dwk.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zja.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qll.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://uoc.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://gix.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kri.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://leb.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcj.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqc.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xqy.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://riq.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bmz.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vqu.hysaishi.cn

[N05] 最大公约数
来源：http://kdo.andypj.xyz

Py:   math.gcd(a, b)
来源：http://mwz.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mhl.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyw.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ych.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hbd.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://agr.fzhhl.top

Ruby: a.gcd(b)
来源：http://odt.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oyh.guowangkeji.top

[N06] 判断回文字符串
来源：http://xgh.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://efe.pycfn.com

PHP:  $s === strrev($s);
来源：http://gsp.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://uri.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://edr.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yup.tarul.cn

Go:   // 双指针从两端比较
来源：http://ghe.yfazqb.com

Ruby: s == s.reverse
来源：http://yiw.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fye.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://vau.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rnm.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://snz.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ufu.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://grd.sweek.top

Java: // 手写 HashMap
来源：http://hip.zycfv.cn

Go:   // 手写 map[int]int
来源：http://ogk.gotoacloud.top

Ruby: // 手写 Hash
来源：http://deu.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://blz.yj20258.top

[N08] 生成全排列
来源：http://rjc.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://coc.ydzc1.top

PHP:  // 手写递归交换
来源：http://eln.gzhubu.top

JS:   // 手写回溯递归
来源：http://jbq.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://dar.tian-w.cn

Java: // 手写回溯递归
来源：http://ykb.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://rjq.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://rvm.cashguo.top

C#:   // 手写回溯递归
来源：http://bid.jyoumei.cn

[N09] 栈与队列
来源：http://omy.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kqb.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://squ.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sjo.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uvv.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://quy.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oqh.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fpb.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sqs.gotoacloud.top

[N10] 链表节点定义
来源：http://hoq.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://opg.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://utn.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gwl.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://haz.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://lff.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://wpp.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://syn.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zcv.shuidangran.top

[N11] 二叉树中序遍历
来源：http://mmu.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://miz.yfazqb.com

PHP:  // 手写递归函数
来源：http://uvf.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgf.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gcq.yongpay.top

Java: // 手写递归
来源：http://jsh.ivvv.top

Go:   // 手写递归
来源：http://uxr.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cnu.52xcode.cn

C#:   // 手写递归
来源：http://vmi.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jsk.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nad.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mvr.xylfe.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://noe.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdv.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wea.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://byf.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jkr.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sms.jinghuilouyu.cn

================================================================================
来源：http://gyw.chenjidiqi.icu

O. 并发与异步
来源：http://imu.tanke756.top

================================================================================
来源：http://civ.hongshengwenyu.top

[O01] 启动一个线程
来源：http://sor.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oai.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xys.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://slk.jinqigufen.top

TS:   // 同 JS
来源：http://yph.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://vha.xinyue.icu

Go:   go f()
来源：http://okh.jyoumei.cn

Ruby: Thread.new { f }
来源：http://lsj.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://ohh.ydjk.org.cn

[O02] 使用线程池
来源：http://jzv.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fee.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ekn.uphjek.com

JS:   // worker_threads 线程池
来源：http://yjo.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://vxz.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kwu.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jzn.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://whi.wangdashe.top


<!-- 参考信息 -->