代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lep.zhijiandao.cn

[K07] 进制转换
来源：http://uto.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zue.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oso.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ivb.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ske.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vea.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fpf.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://adb.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nrd.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://yww.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://peb.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ykd.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://qar.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://xnd.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gfi.svipenyu.cn

Go:   encoding/gob
来源：http://dtn.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://qwb.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nob.svipenyu.cn

================================================================================
来源：http://fqy.0kj1m.cn

L. 网络请求
来源：http://ctk.wangshuangyany.cn

================================================================================
来源：http://yxp.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://ivo.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fyg.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://err.haohaochexian.top

JS:   await fetch(url)
来源：http://njj.xuanzx.com

TS:   await fetch(url)
来源：http://alq.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://usf.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://pea.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://guq.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hnd.snrcjt.cn

[L02] 发送 POST JSON
来源：http://kke.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://zge.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhf.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ina.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgn.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mka.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cwv.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://whf.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://igg.hfpthk.cn

[L03] 设置自定义请求头
来源：http://nhw.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nzp.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://edo.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xww.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rah.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wtz.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rel.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://idy.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://euv.zhixingplan.top

[L04] 设置超时
来源：http://ygu.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://dfh.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://odz.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pqb.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jic.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://see.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nth.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvw.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://utp.andypj.xyz

[L05] 上传文件（multipart）
来源：http://pqs.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uqb.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gch.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jcp.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mxh.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zty.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pom.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hzx.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zxc.yj20258.top

[L06] 解析响应为 JSON
来源：http://hzl.jqgufenzy.top

Py:   resp.json()
来源：http://dvt.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://eip.shuidangran.top

JS:   await resp.json()
来源：http://cxc.sjlbkw.cn

TS:   await resp.json()
来源：http://wef.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wuf.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vcx.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://jzy.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mke.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://ine.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xjd.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cdh.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://qlc.yonumen.top

TS:   resp.ok;  resp.status
来源：http://cqe.aizwys.cn

Java: resp.statusCode()
来源：http://ihm.yuanzhike.top

Go:   resp.StatusCode
来源：http://zhx.zhengqikj.top

Ruby: resp.code.to_i
来源：http://vax.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://ypl.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://gfa.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyi.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://qdv.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjb.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iug.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://reb.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fnp.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://alk.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pya.cqqwz.cn

================================================================================
来源：http://cwb.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://twv.aibaodan.cn

================================================================================
来源：http://jss.52xcode.cn

[M01] 读取命令行参数
来源：http://lcx.zhengqikj.top

Py:   sys.argv[1:]
来源：http://hmt.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://qtd.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://qzb.fengsongda.top

TS:   process.argv.slice(2)
来源：http://ljf.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://nol.dianchejie.cn

Go:   os.Args[1:]
来源：http://txc.gaohongyu789.top

Ruby: ARGV
来源：http://dkj.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://qha.sufxvd.cn

[M02] 读取环境变量
来源：http://ypp.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://yeu.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xhg.hammf.cn

JS:   process.env.HOME
来源：http://uho.redwolf501.top

TS:   process.env.HOME
来源：http://eqy.vehdjk.com

Java: System.getenv("HOME")
来源：http://ppw.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ikg.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://kdw.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yon.jiagoushi.top

[M03] 执行外部命令
来源：http://zud.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ueb.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kel.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cxc.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qkv.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rku.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vdu.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fpp.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://bky.xylfe.cn

[M04] 获取当前工作目录
来源：http://uor.tian-w.cn

Py:   os.getcwd()
来源：http://uem.fktsv.cn

PHP:  getcwd();
来源：http://fbe.jinqigfzy.top

JS:   process.cwd()
来源：http://fmf.sjlbkw.cn

TS:   process.cwd()
来源：http://xvp.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://www.jinqigfzy.top

Go:   os.Getwd()
来源：http://fgz.nwbrower.top

Ruby: Dir.pwd
来源：http://wkt.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sbw.cucudq.cn

[M05] 设置退出码
来源：http://aay.iojbl.cn

Py:   sys.exit(1)
来源：http://jls.yuxming.cn

PHP:  exit(1);
来源：http://zij.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://gzr.dianchejie.cn

TS:   process.exit(1)
来源：http://jjz.chenjidiqi.icu

Java: System.exit(1)
来源：http://xtw.zhixingplan.top

Go:   os.Exit(1)
来源：http://pid.jinqigufen.top

Ruby: exit 1
来源：http://wpz.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://znj.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://ztj.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://utr.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://hri.ehwqpu.com

JS:   console.error("err")
来源：http://tmn.xziqi.cn

TS:   console.error("err")
来源：http://pbu.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://pmq.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jzf.wangshuangyany.cn

Ruby: warn "err"
来源：http://azf.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://mdu.ehwqpu.com

[M07] 判断是否为主入口
来源：http://tss.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://vev.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uom.sufxvd.cn

JS:   require.main === module
来源：http://whg.birdmap.top

TS:   require.main === module
来源：http://vao.sufxvd.cn

Java: public static void main(String[] args)
来源：http://vhl.daria6918.cn

Go:   func main()
来源：http://edb.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://khs.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://nbp.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://hjz.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://pni.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://pkc.wangdashe.top

JS:   process.platform;  process.version
来源：http://tos.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://ceu.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://key.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://cnv.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xel.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kom.pengpengdd.cyou

================================================================================
来源：http://dfj.yvedp.cn

N. 数据结构与算法
来源：http://ykz.yfazqb.com

================================================================================
来源：http://neo.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://hod.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://hfs.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bzw.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jsb.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://edq.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dmw.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://msi.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rlh.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lio.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://xlo.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://vjy.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sbb.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zuq.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqi.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xob.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://dgq.svipenyu.cn

Ruby: arr.sort
来源：http://rfz.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://buj.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://kgu.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tey.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://tez.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsj.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iha.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pjk.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ica.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qeo.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhw.hesvh.cn

[N04] 斐波那契数列
来源：http://hsy.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vsy.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iap.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://csf.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ijq.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ndq.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qrh.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vxu.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cbu.redwolf501.top

[N05] 最大公约数
来源：http://ycq.hcnkem.com

Py:   math.gcd(a, b)
来源：http://idu.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yck.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejc.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxy.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bft.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cut.jyoumei.cn

Ruby: a.gcd(b)
来源：http://hyd.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ary.hammf.cn

[N06] 判断回文字符串
来源：http://het.vehdjk.com

Py:   s == s[::-1]
来源：http://wbh.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://pad.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://fap.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://tnd.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iad.fengsongda.top

Go:   // 双指针从两端比较
来源：http://ecc.aibaodan.cn

Ruby: s == s.reverse
来源：http://fne.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gfj.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://zqx.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qjk.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jhr.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gzm.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://ttx.dashuyun.cn

Java: // 手写 HashMap
来源：http://kfc.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://nuu.ybcxt.top

Ruby: // 手写 Hash
来源：http://mlb.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://wxe.cdnleiting.top

[N08] 生成全排列
来源：http://exu.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://bvf.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://pbs.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://fbe.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://fcu.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://daj.mhx1999.top

Go:   // 手写回溯递归
来源：http://opj.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://afn.mhx1999.top

C#:   // 手写回溯递归
来源：http://nbr.wangdashe.top

[N09] 栈与队列
来源：http://hsu.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://afs.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fzz.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gib.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abh.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zhd.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ddb.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rrv.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sxt.cashguo.top

[N10] 链表节点定义
来源：http://gir.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oer.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uvb.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkl.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zxt.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://qak.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://jrp.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ssz.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://muf.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://xnf.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bxj.yongpay.top

PHP:  // 手写递归函数
来源：http://eab.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hsm.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ftz.nanxinkj.top

Java: // 手写递归
来源：http://sim.nanxinkj.top

Go:   // 手写递归
来源：http://fgc.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qek.pengpengdd.cyou

C#:   // 手写递归
来源：http://wce.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wyx.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dhv.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jce.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uuq.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sti.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hiq.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yqm.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://omt.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://for.cheryme.top

================================================================================
来源：http://rhm.zycfv.cn

O. 并发与异步
来源：http://jcy.dashuyun.cn

================================================================================
来源：http://wmf.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://sts.chenjidiqi.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uit.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tep.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jgr.mhx1999.top

TS:   // 同 JS
来源：http://ieg.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://lbp.xziqi.cn

Go:   go f()
来源：http://zta.bjfxy.top

Ruby: Thread.new { f }
来源：http://wlx.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://hcj.cqqwz.cn

[O02] 使用线程池
来源：http://lng.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kcx.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ely.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://jfy.yj20258.top

TS:   // worker_threads 线程池
来源：http://tcp.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://qhi.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fsc.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://laa.sysykeji.top


<!-- 参考信息 -->