代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kba.bjfxy.top

[K07] 进制转换
来源：http://gtn.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ati.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://las.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jug.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://def.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://amv.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://boq.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zou.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://koc.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://cbj.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://stw.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kca.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://kwo.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://dho.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bxe.chenlongwang.top

Go:   encoding/gob
来源：http://jhp.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://qbt.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jvu.birdmap.top

================================================================================
来源：http://pgh.quarkkingdee.top

L. 网络请求
来源：http://nkx.mhx1999.top

================================================================================
来源：http://bie.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://yuf.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xww.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fje.ivvv.top

JS:   await fetch(url)
来源：http://bgs.hnqzz.top

TS:   await fetch(url)
来源：http://vak.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ego.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://nte.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zdu.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://shv.hysaishi.cn

[L02] 发送 POST JSON
来源：http://fmm.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://nxf.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://apc.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dik.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifm.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tia.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nip.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uok.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dol.ivvv.top

[L03] 设置自定义请求头
来源：http://wjd.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fvt.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dfq.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpb.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://upj.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://adh.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ham.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iks.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahj.ywan-chungtsiang.top

[L04] 设置超时
来源：http://ayp.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://tum.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wkr.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oot.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://orf.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://seg.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xol.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rab.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://frj.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://jea.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sld.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqo.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fxg.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qwg.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vbx.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bbe.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://soj.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tdd.birdmap.top

[L06] 解析响应为 JSON
来源：http://kvh.ctjpmb.com

Py:   resp.json()
来源：http://pyp.c1oappe.top

PHP:  json_decode($body, true);
来源：http://prz.tanke756.top

JS:   await resp.json()
来源：http://ohv.zdbjq.cn

TS:   await resp.json()
来源：http://qdu.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://spv.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ise.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://bmg.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bfz.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://gle.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gum.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cqx.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://zln.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://jhi.mhx1999.top

Java: resp.statusCode()
来源：http://kic.gotoacloud.top

Go:   resp.StatusCode
来源：http://uxg.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://wql.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://qgj.hysaishi.cn

[L08] 并发请求多个地址
来源：http://dxe.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oos.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://omz.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etj.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qbl.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ime.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dmg.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aoo.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cyu.zhoulong.xyz

================================================================================
来源：http://req.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://vhd.zhiwuduotai.top

================================================================================
来源：http://ijj.gogol.net.cn

[M01] 读取命令行参数
来源：http://vyd.svipenyu.cn

Py:   sys.argv[1:]
来源：http://ijp.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://tep.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://gpg.pycfn.com

TS:   process.argv.slice(2)
来源：http://xpa.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://cyg.guannengcc.top

Go:   os.Args[1:]
来源：http://pdo.0kj1m.cn

Ruby: ARGV
来源：http://odb.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://hwr.nanxinkj.top

[M02] 读取环境变量
来源：http://vio.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://ehi.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://unj.hywenlv.cn

JS:   process.env.HOME
来源：http://bwk.xylfe.cn

TS:   process.env.HOME
来源：http://sys.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://qgl.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ewn.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://shg.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kfx.redwolf501.top

[M03] 执行外部命令
来源：http://cne.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jbi.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://otw.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sqf.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gsq.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://szo.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://laf.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iic.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://sec.cqqwz.cn

[M04] 获取当前工作目录
来源：http://zmj.sxryk.cn

Py:   os.getcwd()
来源：http://atb.wangdashe.top

PHP:  getcwd();
来源：http://ogw.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://sdw.xuanzx.com

TS:   process.cwd()
来源：http://vnk.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://upk.cdnleiting.top

Go:   os.Getwd()
来源：http://jxu.jqgfzy.top

Ruby: Dir.pwd
来源：http://dzi.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://jih.hywenlv.cn

[M05] 设置退出码
来源：http://kkh.zhoulong.xyz

Py:   sys.exit(1)
来源：http://cgv.yuanzhike.top

PHP:  exit(1);
来源：http://dfk.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://xoo.gotoacloud.top

TS:   process.exit(1)
来源：http://txc.daxiang520.top

Java: System.exit(1)
来源：http://yav.dashuyun.cn

Go:   os.Exit(1)
来源：http://pno.xinyue.icu

Ruby: exit 1
来源：http://vnr.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dfj.chenzaomai.com

[M06] 向标准错误输出
来源：http://mzo.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://eyo.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://qsh.zhijiandao.cn

JS:   console.error("err")
来源：http://jsa.sxryk.cn

TS:   console.error("err")
来源：http://omg.havefunace.top

Java: System.err.println("err")
来源：http://ovy.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ymo.zhoulong.xyz

Ruby: warn "err"
来源：http://npw.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://sgl.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://jmq.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://msb.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oya.yj20258.top

JS:   require.main === module
来源：http://lfg.feifeiyinyue.top

TS:   require.main === module
来源：http://vzi.birdmap.top

Java: public static void main(String[] args)
来源：http://nxg.daria6918.cn

Go:   func main()
来源：http://asc.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pgr.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://kam.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://bgy.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://juo.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://lbz.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://vhg.aibaodan.cn

TS:   process.platform;  process.version
来源：http://fph.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnf.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ete.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tfq.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://aqh.wangshuangyany.cn

================================================================================
来源：http://gpc.guannengcc.top

N. 数据结构与算法
来源：http://kox.yongpay.top

================================================================================
来源：http://ayu.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://eww.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xbw.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dny.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tor.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgw.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zlm.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://kqn.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://yxc.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dqg.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://pfo.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://vxf.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://apt.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bnp.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nvg.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://chm.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://dil.hfpthk.cn

Ruby: arr.sort
来源：http://qua.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ntg.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://nmu.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://szb.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://cyt.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aha.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vhk.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wxr.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bif.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jkk.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://cxk.jyoumei.cn

[N04] 斐波那契数列
来源：http://jep.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pib.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xdf.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bxb.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yla.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jru.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zuj.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vdf.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kyu.snrcjt.cn

[N05] 最大公约数
来源：http://klq.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://gvv.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://his.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btj.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bib.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itu.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cky.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://ata.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bah.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://qqi.ydjk.org.cn

Py:   s == s[::-1]
来源：http://jud.birdmap.top

PHP:  $s === strrev($s);
来源：http://wmd.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://rem.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://hxq.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ebo.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://qce.jqgfzy.top

Ruby: s == s.reverse
来源：http://kjr.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bns.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://akg.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jpp.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ajh.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qyp.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://vxu.gzhubu.top

Java: // 手写 HashMap
来源：http://olr.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://bxt.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://ooi.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://pjn.dashuyun.cn

[N08] 生成全排列
来源：http://bfr.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://iwa.gotoacloud.top

PHP:  // 手写递归交换
来源：http://ohc.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://wrc.ehwqpu.com

TS:   // 手写回溯递归
来源：http://syv.wangdashe.top

Java: // 手写回溯递归
来源：http://fne.0kj1m.cn

Go:   // 手写回溯递归
来源：http://npo.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://djm.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://zyh.nanxinkj.top

[N09] 栈与队列
来源：http://dym.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://khr.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://duf.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mbu.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ibb.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ouu.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uoz.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nir.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pdk.nanxinkj.top

[N10] 链表节点定义
来源：http://wdv.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wqw.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ale.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hjd.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jwc.316326.xyz

Java: class Node { int v; Node next; }
来源：http://wxp.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://loy.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://peo.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jwc.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://msb.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kav.hywenlv.cn

PHP:  // 手写递归函数
来源：http://blo.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://icj.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpc.yangfankeji.com

Java: // 手写递归
来源：http://yxz.jqgfzy.top

Go:   // 手写递归
来源：http://nbl.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iww.ivvv.top

C#:   // 手写递归
来源：http://wie.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ssc.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oan.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rcz.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baq.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxx.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tjb.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ddm.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cpy.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://moj.hongshengwenyu.top

================================================================================
来源：http://tol.ivvv.top

O. 并发与异步
来源：http://zce.xylfe.cn

================================================================================
来源：http://ezc.yfazqb.com

[O01] 启动一个线程
来源：http://xjm.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xgv.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oqw.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jau.jinqigfzy.top

TS:   // 同 JS
来源：http://yvf.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://nnl.kuanghao11.cn

Go:   go f()
来源：http://bya.ybcxt.top

Ruby: Thread.new { f }
来源：http://oro.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://hjb.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://far.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dwa.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mhh.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://elj.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://mqm.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://zjd.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cdk.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pwv.ctjpmb.com


<!-- 参考信息 -->