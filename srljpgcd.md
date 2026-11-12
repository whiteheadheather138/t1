代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fiv.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ejr.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fas.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lum.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oan.guannengcc.top

[K07] 进制转换
来源：http://bfc.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lza.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evq.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yxu.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yso.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eeg.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kux.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zaj.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hll.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://ryh.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://wrw.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yzd.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://rhm.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://sdl.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vlo.havefunace.top

Go:   encoding/gob
来源：http://wlb.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://oio.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pmr.shanyushiyangtech.top

================================================================================
来源：http://rwg.epnwcf.com

L. 网络请求
来源：http://vxg.yangfankeji.com

================================================================================
来源：http://wjp.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://xdr.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qhh.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jge.cheryme.top

JS:   await fetch(url)
来源：http://kfh.snrcjt.cn

TS:   await fetch(url)
来源：http://wpi.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://keu.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://bse.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yqa.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lgu.gogol.net.cn

[L02] 发送 POST JSON
来源：http://hcx.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://oxo.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://viw.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rdw.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osw.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kha.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xwq.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfe.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhj.havefunace.top

[L03] 设置自定义请求头
来源：http://fax.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vfr.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cco.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxm.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qbo.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iee.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tca.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ywt.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yxy.kuanghao11.cn

[L04] 设置超时
来源：http://bhx.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://ogf.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qtk.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hwy.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hec.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://esl.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://efa.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sbk.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdq.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://wik.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://els.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dzl.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mfw.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tdw.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fzw.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tyo.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cho.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpx.cheryme.top

[L06] 解析响应为 JSON
来源：http://abz.shanyushiyangkeji.top

Py:   resp.json()
来源：http://zmg.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://zdb.xziqi.cn

JS:   await resp.json()
来源：http://jrj.quarkkingdee.top

TS:   await resp.json()
来源：http://ujj.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wvf.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ixs.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://ltc.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oys.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://dei.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ncx.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://buo.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://wes.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://pcz.shangyingyoupin.top

Java: resp.statusCode()
来源：http://dsl.cucudq.cn

Go:   resp.StatusCode
来源：http://xmd.aibaodan.cn

Ruby: resp.code.to_i
来源：http://pcb.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://svu.c1oappe.top

[L08] 并发请求多个地址
来源：http://jad.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fve.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://tmc.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://syh.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lac.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fhe.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qbz.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ahp.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jld.yueranfly.top

================================================================================
来源：http://dfp.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://erj.jiagoushi.top

================================================================================
来源：http://bsy.snrcjt.cn

[M01] 读取命令行参数
来源：http://kdw.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://nuo.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://nnx.hammf.cn

JS:   process.argv.slice(2)
来源：http://zaq.meibo888.top

TS:   process.argv.slice(2)
来源：http://sdj.havefunace.top

Java: args 数组（main 方法参数）
来源：http://wwh.chenzaomai.com

Go:   os.Args[1:]
来源：http://jau.yj20258.top

Ruby: ARGV
来源：http://rwz.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://uph.tarul.cn

[M02] 读取环境变量
来源：http://sxe.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://xms.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://anp.cqqwz.cn

JS:   process.env.HOME
来源：http://ehu.hfpthk.cn

TS:   process.env.HOME
来源：http://vlj.sxryk.cn

Java: System.getenv("HOME")
来源：http://wzv.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gzf.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://cgq.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qvd.uphjek.com

[M03] 执行外部命令
来源：http://met.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ppz.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lld.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qrb.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vny.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ycs.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qkj.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://rye.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://urx.shuidangran.top

[M04] 获取当前工作目录
来源：http://ccx.jiagoushi.top

Py:   os.getcwd()
来源：http://fvh.ivvv.top

PHP:  getcwd();
来源：http://dco.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://zep.zhengqikj.top

TS:   process.cwd()
来源：http://tws.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://lys.gaohongyu789.top

Go:   os.Getwd()
来源：http://nmf.redwolf501.top

Ruby: Dir.pwd
来源：http://lci.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://eon.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://ssc.ppjwa.cn

Py:   sys.exit(1)
来源：http://dtx.sjlbkw.cn

PHP:  exit(1);
来源：http://kax.sysykeji.top

JS:   process.exit(1)
来源：http://oqt.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://yvq.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://btb.fzhhl.top

Go:   os.Exit(1)
来源：http://txg.dianchejie.cn

Ruby: exit 1
来源：http://dqg.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gdh.wangdashe.top

[M06] 向标准错误输出
来源：http://qjg.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://rhb.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wqh.ivvv.top

JS:   console.error("err")
来源：http://dfu.zhiwuduotai.top

TS:   console.error("err")
来源：http://zmn.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://vvw.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bse.shangyingyoupin.top

Ruby: warn "err"
来源：http://mii.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://zak.yuxming.cn

[M07] 判断是否为主入口
来源：http://tsn.316326.xyz

Py:   if __name__ == "__main__":
来源：http://vxc.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dvi.zhaomingkeji.xyz

JS:   require.main === module
来源：http://bxx.cdnleiting.top

TS:   require.main === module
来源：http://yai.tarul.cn

Java: public static void main(String[] args)
来源：http://cow.ydjk.org.cn

Go:   func main()
来源：http://ith.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sjy.sysykeji.top

C#:   static void Main(string[] args)
来源：http://bvn.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://lqr.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://njj.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://fjf.jyoumei.cn

JS:   process.platform;  process.version
来源：http://fvt.yj202588.top

TS:   process.platform;  process.version
来源：http://ajq.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rwl.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://kjl.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zko.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yio.vqdsnc.cn

================================================================================
来源：http://fcf.cheryme.top

N. 数据结构与算法
来源：http://oqf.cucudq.cn

================================================================================
来源：http://aly.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://pdf.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://tsx.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rgi.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nho.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ivi.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://cxw.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://enr.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eli.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://fcy.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://iwi.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://uem.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dqh.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hqo.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyv.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://epl.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://mnd.jqgufenzy.top

Ruby: arr.sort
来源：http://trd.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kwr.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://grp.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mog.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://lpf.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hbi.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pnw.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wsk.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ikf.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gaq.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vgf.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://kti.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mxh.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tkk.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qtw.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rux.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://umy.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://htt.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cvz.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bek.hysaishi.cn

[N05] 最大公约数
来源：http://dvg.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://vky.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ect.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aqy.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://trq.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ohi.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://doc.meibo888.top

Ruby: a.gcd(b)
来源：http://owh.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xrh.epnwcf.com

[N06] 判断回文字符串
来源：http://she.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://vfm.sysykeji.top

PHP:  $s === strrev($s);
来源：http://qrb.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://hca.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://ldy.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cet.epnwcf.com

Go:   // 双指针从两端比较
来源：http://otk.yj20258888.top

Ruby: s == s.reverse
来源：http://ssm.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zwo.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://nsi.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zso.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rty.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nan.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://vye.fzhhl.top

Java: // 手写 HashMap
来源：http://ttj.yonumen.top

Go:   // 手写 map[int]int
来源：http://aff.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://azu.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://jzj.yj20258888.top

[N08] 生成全排列
来源：http://iwi.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://vtb.yuanzhike.top

PHP:  // 手写递归交换
来源：http://tvp.cashguo.top

JS:   // 手写回溯递归
来源：http://uyk.jqgfzy.top

TS:   // 手写回溯递归
来源：http://the.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://yze.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://rwh.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://wxh.cdnleiting.top

C#:   // 手写回溯递归
来源：http://dwd.iojbl.cn

[N09] 栈与队列
来源：http://ocs.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zjt.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sdl.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://drl.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kyw.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://roh.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zhr.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ize.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uci.bjfxy.top

[N10] 链表节点定义
来源：http://kro.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vmu.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://pbs.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ggl.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zzy.meibo888.top

Java: class Node { int v; Node next; }
来源：http://phz.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://qky.sysykeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xku.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yyy.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://yqz.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ffj.fehbvm.com

PHP:  // 手写递归函数
来源：http://fsw.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gds.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvx.yuxming.cn

Java: // 手写递归
来源：http://bob.jqgfzy.top

Go:   // 手写递归
来源：http://btr.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qbr.yanxiufei.cn

C#:   // 手写递归
来源：http://qcl.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rul.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://owt.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ckw.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zau.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzr.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hrv.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pnn.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hij.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ker.yonumen.top

================================================================================
来源：http://wgq.yj202588.top

O. 并发与异步
来源：http://gls.daria6918.cn

================================================================================
来源：http://zpz.yonumen.top

[O01] 启动一个线程
来源：http://lab.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://edx.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vez.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nkp.zhoulong.xyz

TS:   // 同 JS
来源：http://uio.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://syc.shanyushiyangkeji.top

Go:   go f()
来源：http://pbc.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://geo.yonumen.top

C#:   Task.Run(() => F());
来源：http://vou.sysykeji.top

[O02] 使用线程池
来源：http://jmv.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wcv.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iws.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://ear.sjlbkw.cn


<!-- 参考信息 -->