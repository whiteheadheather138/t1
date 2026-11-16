代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvk.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nhb.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eok.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jwc.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dcf.yj20258888.top

[K07] 进制转换
来源：http://lmv.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rfg.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hvy.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vai.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tsx.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hkc.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oql.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://buh.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yvr.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://stu.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://hix.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zks.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://nrg.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://eim.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rza.daxiang520.top

Go:   encoding/gob
来源：http://fxr.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://bfp.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kfa.nanxinkj.top

================================================================================
来源：http://hlm.nanxinkj.top

L. 网络请求
来源：http://wys.xylfe.cn

================================================================================
来源：http://qvp.fehbvm.com

[L01] 发送 GET 请求
来源：http://oki.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ott.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mpl.chenzaomai.com

JS:   await fetch(url)
来源：http://duw.chenzaomai.com

TS:   await fetch(url)
来源：http://fba.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gpw.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://ook.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://czp.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lrr.sufxvd.cn

[L02] 发送 POST JSON
来源：http://vce.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://bxw.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://huh.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhr.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tcb.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ehb.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zer.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvx.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nan.yuanzhike.top

[L03] 设置自定义请求头
来源：http://qzq.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qcd.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bts.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdu.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wsw.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypj.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bdy.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gkl.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://asw.fehbvm.com

[L04] 设置超时
来源：http://nlf.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://dls.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tfj.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hjz.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejw.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nam.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xvf.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bsd.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tof.yj202588.top

[L05] 上传文件（multipart）
来源：http://yvf.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bed.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogb.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ntl.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsr.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbe.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ony.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://trx.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://syn.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://lve.zhengqikj.top

Py:   resp.json()
来源：http://dub.sxryk.cn

PHP:  json_decode($body, true);
来源：http://lly.daria6918.cn

JS:   await resp.json()
来源：http://bvn.ivvv.top

TS:   await resp.json()
来源：http://qrl.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnd.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sed.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://psd.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gll.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://rkq.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tch.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpk.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://kyp.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://qma.jinqigufen.top

Java: resp.statusCode()
来源：http://kxf.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://arl.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://hjh.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://dod.yueranfly.top

[L08] 并发请求多个地址
来源：http://qbz.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nsq.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://yus.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccz.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wkn.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://atl.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxh.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uda.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ytf.shanyushiyangkeji.top

================================================================================
来源：http://dos.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://xas.shangyingyoupin.top

================================================================================
来源：http://fvz.zdqjudy.top

[M01] 读取命令行参数
来源：http://ygg.9152youxi.cn

Py:   sys.argv[1:]
来源：http://alo.yueranfly.top

PHP:  $argv;  $argc;
来源：http://vab.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://nyy.cucudq.cn

TS:   process.argv.slice(2)
来源：http://nhq.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://ktx.smart0.xyz

Go:   os.Args[1:]
来源：http://gwc.wangdashe.top

Ruby: ARGV
来源：http://xnk.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://ilr.sjlbkw.cn

[M02] 读取环境变量
来源：http://vyd.yonumen.top

Py:   os.environ.get("HOME")
来源：http://swf.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kzk.ctjpmb.com

JS:   process.env.HOME
来源：http://gmz.hysaishi.cn

TS:   process.env.HOME
来源：http://ook.dashuyun.cn

Java: System.getenv("HOME")
来源：http://fux.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zev.cashguo.top

Ruby: ENV["HOME"]
来源：http://rds.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ibv.jqgfzy.top

[M03] 执行外部命令
来源：http://myc.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vxz.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wnu.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://shf.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pfx.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://owe.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vpp.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://enz.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://ivz.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://dau.gzhubu.top

Py:   os.getcwd()
来源：http://mmu.0kj1m.cn

PHP:  getcwd();
来源：http://ybz.hongshengwenyu.top

JS:   process.cwd()
来源：http://cfs.hnxiangtu.top

TS:   process.cwd()
来源：http://nzn.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://kau.fengsongda.top

Go:   os.Getwd()
来源：http://hqv.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://cwq.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://nxg.ctjpmb.com

[M05] 设置退出码
来源：http://xvg.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://ary.guowangkeji.top

PHP:  exit(1);
来源：http://gih.sufxvd.cn

JS:   process.exit(1)
来源：http://tkr.yj20258888.top

TS:   process.exit(1)
来源：http://jsj.jinghuilouyu.cn

Java: System.exit(1)
来源：http://ivp.jyoumei.cn

Go:   os.Exit(1)
来源：http://zxv.ywan-chungtsiang.top

Ruby: exit 1
来源：http://sci.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rty.jinqigufen.top

[M06] 向标准错误输出
来源：http://qru.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://evd.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xkx.dianchejie.cn

JS:   console.error("err")
来源：http://quc.sweek.top

TS:   console.error("err")
来源：http://nzd.yvedp.cn

Java: System.err.println("err")
来源：http://zcw.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jpu.yonumen.top

Ruby: warn "err"
来源：http://cdj.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://gsv.redwolf501.top

[M07] 判断是否为主入口
来源：http://xsv.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://uej.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ccl.kuanghao11.cn

JS:   require.main === module
来源：http://sui.shuidangran.top

TS:   require.main === module
来源：http://ige.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://ctt.daxiang520.top

Go:   func main()
来源：http://nus.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://add.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://yza.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://pgz.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://ina.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://kvs.shzxlz.cn

JS:   process.platform;  process.version
来源：http://qbf.nanxinkj.top

TS:   process.platform;  process.version
来源：http://ctr.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xnc.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://amv.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rsm.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ecp.sufxvd.cn

================================================================================
来源：http://ihp.hnqzz.top

N. 数据结构与算法
来源：http://ufj.havefunace.top

================================================================================
来源：http://xji.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://gzo.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gwo.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kij.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nqz.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://twf.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://gpf.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://mab.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://avs.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dsi.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://bgm.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://wsn.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pcg.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sir.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qkc.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wue.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://yts.chenlongwang.top

Ruby: arr.sort
来源：http://ubf.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yiw.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://jhu.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cng.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://rfd.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://php.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tck.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btv.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://djf.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://red.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rqz.wangdashe.top

[N04] 斐波那契数列
来源：http://bib.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nhx.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vde.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prs.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ndz.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kir.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lzk.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://drk.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://diy.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://eid.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://xow.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bcg.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yob.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vce.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dnj.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cbo.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://maq.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cga.hcnkem.com

[N06] 判断回文字符串
来源：http://nkt.xziqi.cn

Py:   s == s[::-1]
来源：http://cno.mhx1999.top

PHP:  $s === strrev($s);
来源：http://ewm.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://sfv.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://ihn.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pqp.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://fsi.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://jwb.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pwq.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://ioi.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ook.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://efy.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://onx.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://cbk.zdqjudy.top

Java: // 手写 HashMap
来源：http://fts.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://gtf.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://scu.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://tpt.wangshuangyany.cn

[N08] 生成全排列
来源：http://brb.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://vgs.zhengqikj.top

PHP:  // 手写递归交换
来源：http://dxq.yvedp.cn

JS:   // 手写回溯递归
来源：http://opq.zhixingplan.top

TS:   // 手写回溯递归
来源：http://ejy.quarkkingdee.top

Java: // 手写回溯递归
来源：http://fcq.tarul.cn

Go:   // 手写回溯递归
来源：http://znn.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://cbn.chenlongwang.top

C#:   // 手写回溯递归
来源：http://axg.jyoumei.cn

[N09] 栈与队列
来源：http://yta.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mbt.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qft.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://efe.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aja.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wum.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://snt.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wds.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pkn.yueranfly.top

[N10] 链表节点定义
来源：http://ihe.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvg.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yda.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zec.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oyj.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://ubp.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://mgr.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ecb.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vgh.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://nzi.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zvd.0kj1m.cn

PHP:  // 手写递归函数
来源：http://hwv.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ghd.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xai.xziqi.cn

Java: // 手写递归
来源：http://ouu.yj20258888.top

Go:   // 手写递归
来源：http://wph.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fsu.dashuyun.cn

C#:   // 手写递归
来源：http://wrq.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://teb.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zyv.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xgs.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://huj.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbi.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tpa.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gma.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://thi.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dpd.quarkkingdee.top

================================================================================
来源：http://ykg.hysaishi.cn

O. 并发与异步
来源：http://erq.yuxming.cn

================================================================================
来源：http://xsc.jianghu66.top

[O01] 启动一个线程
来源：http://coq.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lef.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fby.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fer.chenzaomai.com

TS:   // 同 JS
来源：http://bbn.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://ixm.daxiang520.top

Go:   go f()
来源：http://pfd.ctjpmb.com

Ruby: Thread.new { f }
来源：http://fch.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://osv.feifeiyinyue.top

[O02] 使用线程池
来源：http://xiw.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ruv.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eiz.yuxming.cn

JS:   // worker_threads 线程池
来源：http://uhc.jinyuanbaomall.cn


<!-- 参考信息 -->