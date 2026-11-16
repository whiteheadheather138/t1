代发 wailian999

[K06] 解析 URL 查询串
来源：http://acw.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wde.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mhc.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bzr.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tun.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vlq.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bbf.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://syv.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gtf.xylfe.cn

[K07] 进制转换
来源：http://juu.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://anh.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wtk.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cmn.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uid.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://btn.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ygt.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baw.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://irk.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://jmh.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://xpl.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wzn.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://bod.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://pgc.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bto.zdbjq.cn

Go:   encoding/gob
来源：http://zuf.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://msk.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cez.zhiwuduotai.top

================================================================================
来源：http://wyy.shanyushiyangtech.top

L. 网络请求
来源：http://ecq.jinqigufen.top

================================================================================
来源：http://ypw.uphjek.com

[L01] 发送 GET 请求
来源：http://bzh.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xem.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://egg.sweek.top

JS:   await fetch(url)
来源：http://kvk.sysykeji.top

TS:   await fetch(url)
来源：http://stt.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jet.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://mbh.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ojk.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bhj.shuidangran.top

[L02] 发送 POST JSON
来源：http://cai.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yyl.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wfr.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfk.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scm.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tlw.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qqi.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qaj.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwi.bjfxy.top

[L03] 设置自定义请求头
来源：http://dhi.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhr.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sif.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emg.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wvv.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wki.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cns.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sth.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uev.kuanghao11.cn

[L04] 设置超时
来源：http://whi.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://jes.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jss.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izc.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gpz.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://why.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lww.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcn.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hqx.yvedp.cn

[L05] 上传文件（multipart）
来源：http://vio.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dmv.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mdh.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://frr.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ukh.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lih.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hqv.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ftp.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqj.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://eus.hfpthk.cn

Py:   resp.json()
来源：http://lte.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://amn.guannengcc.top

JS:   await resp.json()
来源：http://tgu.jyoumei.cn

TS:   await resp.json()
来源：http://jjz.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vkd.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tto.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://kry.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvq.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://urq.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zlx.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nkt.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://eud.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://lop.smart0.xyz

Java: resp.statusCode()
来源：http://kbx.zhixingplan.top

Go:   resp.StatusCode
来源：http://rku.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://wuj.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://com.sxryk.cn

[L08] 并发请求多个地址
来源：http://fbh.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aob.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://uaj.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wcm.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqa.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ozn.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ucw.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aac.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kbl.ydzc1.top

================================================================================
来源：http://bfz.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://sdv.shanyushiyangtech.top

================================================================================
来源：http://iiv.gzhubu.top

[M01] 读取命令行参数
来源：http://zxx.zhixingplan.top

Py:   sys.argv[1:]
来源：http://egk.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://lfs.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://ane.sysykeji.top

TS:   process.argv.slice(2)
来源：http://rcg.pycfn.com

Java: args 数组（main 方法参数）
来源：http://ilr.guowangkeji.top

Go:   os.Args[1:]
来源：http://mbs.hcnkem.com

Ruby: ARGV
来源：http://wzc.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://tal.dashuyun.cn

[M02] 读取环境变量
来源：http://ufc.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://avi.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wrn.sysykeji.top

JS:   process.env.HOME
来源：http://zud.ybcxt.top

TS:   process.env.HOME
来源：http://kvx.sufxvd.cn

Java: System.getenv("HOME")
来源：http://qnn.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wdp.meibo888.top

Ruby: ENV["HOME"]
来源：http://jbx.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mmn.zhongyouzk.top

[M03] 执行外部命令
来源：http://tbv.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aow.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rny.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sih.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ors.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tqc.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qst.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://upl.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://uef.xinyue.icu

[M04] 获取当前工作目录
来源：http://osg.jianghu66.top

Py:   os.getcwd()
来源：http://oya.zdqjudy.top

PHP:  getcwd();
来源：http://ive.daria6918.cn

JS:   process.cwd()
来源：http://bha.fehbvm.com

TS:   process.cwd()
来源：http://vcc.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://yua.chenzaomai.com

Go:   os.Getwd()
来源：http://nlr.wangdashe.top

Ruby: Dir.pwd
来源：http://wuj.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://jpe.zdbjq.cn

[M05] 设置退出码
来源：http://wct.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://tbn.yuxming.cn

PHP:  exit(1);
来源：http://kpb.jianghu66.top

JS:   process.exit(1)
来源：http://yyz.ydjk.org.cn

TS:   process.exit(1)
来源：http://ofo.shanyushiyangtech.top

Java: System.exit(1)
来源：http://srp.zhixingplan.top

Go:   os.Exit(1)
来源：http://ayz.fanxiaobao.xyz

Ruby: exit 1
来源：http://kyw.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ooh.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://pxv.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://blw.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gdx.mhx1999.top

JS:   console.error("err")
来源：http://wrf.hongshengwenyu.top

TS:   console.error("err")
来源：http://rvf.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://yoo.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pfw.havefunace.top

Ruby: warn "err"
来源：http://ziy.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://ibz.nwbrower.top

[M07] 判断是否为主入口
来源：http://yba.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://ksn.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xfw.quarkkingdee.top

JS:   require.main === module
来源：http://xrg.tian-w.cn

TS:   require.main === module
来源：http://bru.hfpthk.cn

Java: public static void main(String[] args)
来源：http://mgi.shanyushiyangtech.top

Go:   func main()
来源：http://ymb.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hyi.cheryme.top

C#:   static void Main(string[] args)
来源：http://wff.ivvv.top

[M08] 获取系统与运行时信息
来源：http://ixr.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://wnc.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://dzf.dashuyun.cn

JS:   process.platform;  process.version
来源：http://rel.52xcode.cn

TS:   process.platform;  process.version
来源：http://otg.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xrr.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xlw.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tli.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wff.zhoulong.xyz

================================================================================
来源：http://ggt.jianghu66.top

N. 数据结构与算法
来源：http://klm.cheryme.top

================================================================================
来源：http://cwk.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://okh.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://elk.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aoc.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nkk.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bqs.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aii.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://zlg.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zye.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://slw.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://wkx.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://yzo.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ctt.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kep.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rud.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yos.yj202588.top

Go:   slices.Sort(arr)
来源：http://yao.0kj1m.cn

Ruby: arr.sort
来源：http://lob.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgw.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://amy.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jot.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://ahk.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pab.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbu.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwu.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpb.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://isk.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://jnf.hfpthk.cn

[N04] 斐波那契数列
来源：http://jsd.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ijv.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://imw.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zvd.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdx.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uuy.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mdp.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uqi.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ltq.9152youxi.cn

[N05] 最大公约数
来源：http://hpc.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://xck.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mkf.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fjs.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://abh.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zoq.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qdx.uphjek.com

Ruby: a.gcd(b)
来源：http://mgl.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gmo.andypj.xyz

[N06] 判断回文字符串
来源：http://bwp.jqgufenzy.top

Py:   s == s[::-1]
来源：http://kpv.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://ivm.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://zjc.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://nco.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gon.sweek.top

Go:   // 双指针从两端比较
来源：http://zjq.hesvh.cn

Ruby: s == s.reverse
来源：http://qde.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://geg.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://bsf.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bzf.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://njl.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hdd.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://gls.yonumen.top

Java: // 手写 HashMap
来源：http://dak.fehbvm.com

Go:   // 手写 map[int]int
来源：http://auf.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://ucz.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gdj.tanke756.top

[N08] 生成全排列
来源：http://ykd.yj20258.top

Py:   itertools.permutations(arr)
来源：http://xxs.chenlongwang.top

PHP:  // 手写递归交换
来源：http://voh.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://zew.yuxming.cn

TS:   // 手写回溯递归
来源：http://jey.jinqigfzy.top

Java: // 手写回溯递归
来源：http://guy.jqgfzy.top

Go:   // 手写回溯递归
来源：http://eru.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://kqm.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://fbt.meibo888.top

[N09] 栈与队列
来源：http://wba.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sny.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vvi.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pah.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abh.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jpy.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dpv.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvr.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jsl.hnqzz.top

[N10] 链表节点定义
来源：http://qsr.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pyy.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tef.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://svy.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zew.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://uff.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://ubl.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ihr.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nbd.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://uhl.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ben.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://yam.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yfr.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mim.andypj.xyz

Java: // 手写递归
来源：http://vlp.hfpthk.cn

Go:   // 手写递归
来源：http://yar.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dgl.hcnkem.com

C#:   // 手写递归
来源：http://kpy.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tly.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhg.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hif.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://djx.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwt.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fyr.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mkf.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ypk.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qyp.ydzc1.top

================================================================================
来源：http://pad.xuanzx.com

O. 并发与异步
来源：http://xhx.zhengqikj.top

================================================================================
来源：http://ipd.shzxlz.cn

[O01] 启动一个线程
来源：http://auc.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jvv.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vry.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sor.svipenyu.cn

TS:   // 同 JS
来源：http://aks.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://bep.ppjwa.cn

Go:   go f()
来源：http://wvk.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://dlr.yj202588.top

C#:   Task.Run(() => F());
来源：http://tuh.0kj1m.cn


<!-- 参考信息 -->