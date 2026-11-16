代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cqj.zhaomingkeji.xyz

[K07] 进制转换
来源：http://igm.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vvw.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://heh.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qja.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vmh.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sit.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kkv.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ayp.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://spj.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://yql.cashguo.top

Py:   pickle.dumps(obj)
来源：http://sax.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lip.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://szv.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://ayi.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cmb.tanke756.top

Go:   encoding/gob
来源：http://rsh.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://wbu.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://enx.mhx1999.top

================================================================================
来源：http://xny.yj20258.top

L. 网络请求
来源：http://mln.ywan-chungtsiang.top

================================================================================
来源：http://wrj.gzhubu.top

[L01] 发送 GET 请求
来源：http://rmp.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://seu.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lwm.sysykeji.top

JS:   await fetch(url)
来源：http://vqn.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://qeh.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tzn.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://ygi.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xze.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eut.mhx1999.top

[L02] 发送 POST JSON
来源：http://ilu.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://dvi.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hkj.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hbl.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jsf.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://enr.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://acs.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bqt.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://guj.hesvh.cn

[L03] 设置自定义请求头
来源：http://kwl.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fol.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pny.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ajq.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mnj.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kcd.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rzr.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://twa.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qnm.birdmap.top

[L04] 设置超时
来源：http://mzv.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://hei.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kny.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wan.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxv.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iie.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jxe.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hve.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evr.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://vln.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mkb.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jou.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ijk.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hmk.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qgj.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pkv.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vpt.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gtu.tian-w.cn

[L06] 解析响应为 JSON
来源：http://zpq.jianghu66.top

Py:   resp.json()
来源：http://wtg.tian-w.cn

PHP:  json_decode($body, true);
来源：http://uqj.bbcook.cn

JS:   await resp.json()
来源：http://nmi.c1oappe.top

TS:   await resp.json()
来源：http://afx.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://klb.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://luq.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://zim.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bkg.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://tbs.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bob.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hjy.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://iuw.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://poc.yanxiufei.cn

Java: resp.statusCode()
来源：http://hdx.epnwcf.com

Go:   resp.StatusCode
来源：http://tfq.tanke756.top

Ruby: resp.code.to_i
来源：http://cip.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://svy.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://kvm.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ngc.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://laz.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kyr.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyq.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qdb.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://whu.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xnc.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tiq.daxiang520.top

================================================================================
来源：http://rul.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://bvc.ybcxt.top

================================================================================
来源：http://fwc.bbcook.cn

[M01] 读取命令行参数
来源：http://ypg.tian-w.cn

Py:   sys.argv[1:]
来源：http://vjx.meibo888.top

PHP:  $argv;  $argc;
来源：http://kkr.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://jsy.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://voe.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://ymy.zhongyouzk.top

Go:   os.Args[1:]
来源：http://asg.yuanzhike.top

Ruby: ARGV
来源：http://ldz.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://fma.316326.xyz

[M02] 读取环境变量
来源：http://qjz.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://ltb.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nxk.zdbjq.cn

JS:   process.env.HOME
来源：http://qyh.yongpay.top

TS:   process.env.HOME
来源：http://mmw.vehdjk.com

Java: System.getenv("HOME")
来源：http://wzh.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jpl.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://kgk.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ifa.hesvh.cn

[M03] 执行外部命令
来源：http://dts.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xvn.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://asc.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ckt.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lre.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zzd.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oly.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://luv.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://sih.iojbl.cn

[M04] 获取当前工作目录
来源：http://aer.quarkkingdee.top

Py:   os.getcwd()
来源：http://agl.daria6918.cn

PHP:  getcwd();
来源：http://lmw.0kj1m.cn

JS:   process.cwd()
来源：http://bsy.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://fbx.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://fmc.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://cwo.gzhubu.top

Ruby: Dir.pwd
来源：http://zku.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://dsu.yuxming.cn

[M05] 设置退出码
来源：http://vdg.yonumen.top

Py:   sys.exit(1)
来源：http://fsl.chenjidiqi.icu

PHP:  exit(1);
来源：http://agd.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://lpp.tianlin.xyz

TS:   process.exit(1)
来源：http://hnv.wangdashe.top

Java: System.exit(1)
来源：http://gsq.gogol.net.cn

Go:   os.Exit(1)
来源：http://sne.snrcjt.cn

Ruby: exit 1
来源：http://onx.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://icv.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://oxu.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://mmi.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ell.pycfn.com

JS:   console.error("err")
来源：http://oqq.gzhubu.top

TS:   console.error("err")
来源：http://mhu.hfpthk.cn

Java: System.err.println("err")
来源：http://wzb.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lqi.gogol.net.cn

Ruby: warn "err"
来源：http://jrn.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://qvv.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://sbg.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://iac.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yza.wangshuangyany.cn

JS:   require.main === module
来源：http://cqj.hfpthk.cn

TS:   require.main === module
来源：http://ksf.xuanzx.com

Java: public static void main(String[] args)
来源：http://nsv.shanyushiyangkeji.top

Go:   func main()
来源：http://ueb.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ped.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://lsl.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://akz.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://rio.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://gyu.guowangkeji.top

JS:   process.platform;  process.version
来源：http://mpz.jqgfzy.top

TS:   process.platform;  process.version
来源：http://fol.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oba.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kfp.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fgz.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://osg.nanxinkj.top

================================================================================
来源：http://roi.0kj1m.cn

N. 数据结构与算法
来源：http://und.zycfv.cn

================================================================================
来源：http://iuo.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://ywn.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://aho.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://psh.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyw.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cuu.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xrb.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://gbz.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yis.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://hts.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://acv.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://nca.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tzz.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://exq.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gtc.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwc.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://ucs.316326.xyz

Ruby: arr.sort
来源：http://faw.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rez.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://mkj.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xsz.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://fuy.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqd.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uyu.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://siv.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aao.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xig.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://vrg.zycfv.cn

[N04] 斐波那契数列
来源：http://qfx.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nrx.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vrd.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wvx.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgj.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://smx.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vmf.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxo.tianlin.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znl.yangfankeji.com

[N05] 最大公约数
来源：http://mix.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://dfz.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sao.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aau.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vhb.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lqz.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bya.52xcode.cn

Ruby: a.gcd(b)
来源：http://nvb.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://idk.vehdjk.com

[N06] 判断回文字符串
来源：http://gwz.316326.xyz

Py:   s == s[::-1]
来源：http://ixb.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://dxs.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://epo.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://oex.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yke.cheryme.top

Go:   // 双指针从两端比较
来源：http://urf.meibo888.top

Ruby: s == s.reverse
来源：http://acr.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://udv.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://ynw.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yzv.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wqm.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://roh.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://obm.9152youxi.cn

Java: // 手写 HashMap
来源：http://vhs.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://rbj.hcnkem.com

Ruby: // 手写 Hash
来源：http://kad.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xrf.birdmap.top

[N08] 生成全排列
来源：http://gxp.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://evk.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://uyz.hfpthk.cn

JS:   // 手写回溯递归
来源：http://xou.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://tza.jqgufenzy.top

Java: // 手写回溯递归
来源：http://kkn.ppjwa.cn

Go:   // 手写回溯递归
来源：http://cxm.yj202588.top

Ruby: arr.permutation.to_a
来源：http://igz.pycfn.com

C#:   // 手写回溯递归
来源：http://dqo.zycfv.cn

[N09] 栈与队列
来源：http://cur.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kda.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kkg.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sot.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ire.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kxy.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ihc.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bqo.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xux.jlsjyb.cn

[N10] 链表节点定义
来源：http://quo.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xik.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fau.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sal.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lmm.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://uzu.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://akm.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sgn.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bzu.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://haj.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rcc.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://htg.kuanghao11.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhg.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sin.bjfxy.top

Java: // 手写递归
来源：http://grq.wangdashe.top

Go:   // 手写递归
来源：http://kql.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kla.shzxlz.cn

C#:   // 手写递归
来源：http://bql.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ava.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpn.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mji.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hdg.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bcg.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yvf.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ztv.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wub.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ipf.redwolf501.top

================================================================================
来源：http://jil.chenzaomai.com

O. 并发与异步
来源：http://nvv.vehdjk.com

================================================================================
来源：http://mef.aibaodan.cn

[O01] 启动一个线程
来源：http://pbt.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ows.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://udv.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nld.fehbvm.com

TS:   // 同 JS
来源：http://cmy.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://nyo.zdbjq.cn

Go:   go f()
来源：http://wus.ivvv.top

Ruby: Thread.new { f }
来源：http://zes.mhx1999.top

C#:   Task.Run(() => F());
来源：http://gid.c1oappe.top

[O02] 使用线程池
来源：http://isu.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iyy.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qqc.hnqzz.top

JS:   // worker_threads 线程池
来源：http://rbh.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://kot.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gql.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yty.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gkk.shangyingyoupin.top


<!-- 参考信息 -->