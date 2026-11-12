代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xly.daria6918.cn

[K07] 进制转换
来源：http://nre.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hxr.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gcu.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://caw.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wzh.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ici.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qoo.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nsh.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://boc.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://afx.tarul.cn

Py:   pickle.dumps(obj)
来源：http://wyi.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nrs.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://ozn.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://hfs.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lcm.wangdashe.top

Go:   encoding/gob
来源：http://uaf.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://pkp.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjb.nanxinkj.top

================================================================================
来源：http://hpo.cdnleiting.top

L. 网络请求
来源：http://nmo.cdnleiting.top

================================================================================
来源：http://xxu.sysykeji.top

[L01] 发送 GET 请求
来源：http://syg.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dfp.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tai.zdqjudy.top

JS:   await fetch(url)
来源：http://fnj.ydjk.org.cn

TS:   await fetch(url)
来源：http://pbq.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dvq.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://ydj.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rda.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://env.fktsv.cn

[L02] 发送 POST JSON
来源：http://xsb.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://noy.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wip.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myq.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gif.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yce.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lql.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cep.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ouo.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://iiw.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://alo.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hqr.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rdb.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zik.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zed.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xyp.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rgl.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://itx.redwolf501.top

[L04] 设置超时
来源：http://tfn.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://mza.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mkj.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhn.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aag.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://low.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iok.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cau.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xhd.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://okz.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xpf.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nhb.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dqj.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kec.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ekh.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sst.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jjj.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tzs.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://yev.fktsv.cn

Py:   resp.json()
来源：http://pos.ivvv.top

PHP:  json_decode($body, true);
来源：http://qfi.gotoacloud.top

JS:   await resp.json()
来源：http://oln.ydzc1.top

TS:   await resp.json()
来源：http://abk.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iqi.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eib.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://nwk.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tlt.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://fty.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kby.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rfs.sweek.top

JS:   resp.ok;  resp.status
来源：http://awa.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://bum.zhoulong.xyz

Java: resp.statusCode()
来源：http://tvc.bjfxy.top

Go:   resp.StatusCode
来源：http://ssf.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://siu.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://nfi.fehbvm.com

[L08] 并发请求多个地址
来源：http://pcb.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gqm.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://yxy.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://shh.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cpp.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://akv.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://awb.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zyy.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwp.zhaomingkeji.xyz

================================================================================
来源：http://teh.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://xgp.hcnkem.com

================================================================================
来源：http://hkf.bbcook.cn

[M01] 读取命令行参数
来源：http://ktt.cheryme.top

Py:   sys.argv[1:]
来源：http://ycp.fehbvm.com

PHP:  $argv;  $argc;
来源：http://lid.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://pzl.c1oappe.top

TS:   process.argv.slice(2)
来源：http://vec.sweek.top

Java: args 数组（main 方法参数）
来源：http://phd.yj202588.top

Go:   os.Args[1:]
来源：http://myl.guowangkeji.top

Ruby: ARGV
来源：http://nqx.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://itw.wangdashe.top

[M02] 读取环境变量
来源：http://ixy.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://pyf.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sii.dianchejie.cn

JS:   process.env.HOME
来源：http://kbc.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://mjg.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://uom.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gak.nwbrower.top

Ruby: ENV["HOME"]
来源：http://pfd.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrl.sxryk.cn

[M03] 执行外部命令
来源：http://vpt.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ifw.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yhe.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hwr.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vcv.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vtp.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wqh.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://ipx.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://oco.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://rew.nwbrower.top

Py:   os.getcwd()
来源：http://lov.shanyushiyangtech.top

PHP:  getcwd();
来源：http://cpq.sufxvd.cn

JS:   process.cwd()
来源：http://jkv.havefunace.top

TS:   process.cwd()
来源：http://ihd.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://qea.zdqjudy.top

Go:   os.Getwd()
来源：http://gyx.ivvv.top

Ruby: Dir.pwd
来源：http://dxf.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sfs.bbcook.cn

[M05] 设置退出码
来源：http://kfk.fehbvm.com

Py:   sys.exit(1)
来源：http://wjt.cdnleiting.top

PHP:  exit(1);
来源：http://anz.ppjwa.cn

JS:   process.exit(1)
来源：http://cap.hnqzz.top

TS:   process.exit(1)
来源：http://exr.aibaodan.cn

Java: System.exit(1)
来源：http://bua.yj20258.top

Go:   os.Exit(1)
来源：http://pik.snrcjt.cn

Ruby: exit 1
来源：http://awy.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cdl.cashguo.top

[M06] 向标准错误输出
来源：http://ghl.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://gli.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://zbq.yj202588.top

JS:   console.error("err")
来源：http://igx.tarul.cn

TS:   console.error("err")
来源：http://uiy.wangdashe.top

Java: System.err.println("err")
来源：http://jag.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cmc.zhengqikj.top

Ruby: warn "err"
来源：http://xqs.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://ytb.zdbjq.cn

[M07] 判断是否为主入口
来源：http://tam.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://tko.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kwu.9152youxi.cn

JS:   require.main === module
来源：http://qhd.wangshuangyany.cn

TS:   require.main === module
来源：http://jip.pycfn.com

Java: public static void main(String[] args)
来源：http://jve.ivvv.top

Go:   func main()
来源：http://nwg.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://scc.redwolf501.top

C#:   static void Main(string[] args)
来源：http://whi.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://tqx.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://nwe.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://vzu.aizwys.cn

JS:   process.platform;  process.version
来源：http://hhm.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://hui.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hvi.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mjb.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsv.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dqd.guannengcc.top

================================================================================
来源：http://lkx.xinyue.icu

N. 数据结构与算法
来源：http://hhu.ybcxt.top

================================================================================
来源：http://qra.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://lfs.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gta.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pjt.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://etl.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzm.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://wwl.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://gwq.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ksi.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qbp.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://wae.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://shr.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qol.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://awh.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://plm.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aum.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://rfn.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://yxx.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vvi.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://qpp.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qax.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://zzc.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fju.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kup.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jgv.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gaa.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://shg.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bot.daria6918.cn

[N04] 斐波那契数列
来源：http://pow.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ukq.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xqt.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ixc.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ted.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tku.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uws.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aim.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zxo.wangshuangyany.cn

[N05] 最大公约数
来源：http://xtd.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://jqf.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://urc.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rtg.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yxe.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wbg.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vam.nwbrower.top

Ruby: a.gcd(b)
来源：http://rzk.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nwe.jqgufenzy.top

[N06] 判断回文字符串
来源：http://vzu.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://feq.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://duo.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://ljv.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://yzz.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awt.epnwcf.com

Go:   // 双指针从两端比较
来源：http://mon.hesvh.cn

Ruby: s == s.reverse
来源：http://tiv.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fjm.yj202588.top

[N07] 两数之和（返回下标）
来源：http://mox.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://htd.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eth.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://enh.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://oem.chenzaomai.com

Java: // 手写 HashMap
来源：http://ltq.yfazqb.com

Go:   // 手写 map[int]int
来源：http://ncv.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://zjx.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wwr.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://sdq.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://kky.uphjek.com

PHP:  // 手写递归交换
来源：http://zyz.uphjek.com

JS:   // 手写回溯递归
来源：http://zyi.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://uie.chenlongwang.top

Java: // 手写回溯递归
来源：http://sjz.c1oappe.top

Go:   // 手写回溯递归
来源：http://anp.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://tja.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://uro.zhoulong.xyz

[N09] 栈与队列
来源：http://tbl.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mhd.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agj.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://msp.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yoz.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nps.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vnr.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fok.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ycv.aizwys.cn

[N10] 链表节点定义
来源：http://cyx.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ybl.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jaw.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xro.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tlr.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://jrx.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://kkc.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uwa.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vvd.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://yne.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tkc.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://lqk.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqk.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kon.ehwqpu.com

Java: // 手写递归
来源：http://odf.hcnkem.com

Go:   // 手写递归
来源：http://wqt.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jxg.jyoumei.cn

C#:   // 手写递归
来源：http://ccw.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xyt.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vtr.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gax.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nik.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpd.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oxl.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rmm.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eax.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pzh.zhaomingkeji.xyz

================================================================================
来源：http://icw.havefunace.top

O. 并发与异步
来源：http://qrs.cucudq.cn

================================================================================
来源：http://hlk.cdnleiting.top

[O01] 启动一个线程
来源：http://rfg.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ado.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tay.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://esg.dashuyun.cn

TS:   // 同 JS
来源：http://qiu.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://svg.nwbrower.top

Go:   go f()
来源：http://qeh.yuxming.cn

Ruby: Thread.new { f }
来源：http://fph.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://lcq.ctjpmb.com

[O02] 使用线程池
来源：http://fgt.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dih.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lwj.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://vle.sxryk.cn

TS:   // worker_threads 线程池
来源：http://ivb.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cig.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mtq.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rky.fehbvm.com


<!-- 参考信息 -->