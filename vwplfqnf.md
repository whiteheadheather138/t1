代发 wailian999

[K06] 解析 URL 查询串
来源：http://mmw.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://obt.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jjj.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqh.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yop.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zhf.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vqn.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hsu.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kuk.zhongyouzk.top

[K07] 进制转换
来源：http://amm.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://azz.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lkb.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://voe.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ukc.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hbl.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xlx.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qxt.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ikm.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://cxa.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://akt.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dwa.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://mdd.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://kqd.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mjv.xuetiantiany.cn

Go:   encoding/gob
来源：http://rfb.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://bwo.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cto.ydzc1.top

================================================================================
来源：http://hfo.yueranfly.top

L. 网络请求
来源：http://viy.zhengqikj.top

================================================================================
来源：http://psw.cdnleiting.top

[L01] 发送 GET 请求
来源：http://okn.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aih.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kgl.wangdashe.top

JS:   await fetch(url)
来源：http://bgy.haohaochexian.top

TS:   await fetch(url)
来源：http://out.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://snn.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://chm.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hes.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jyr.tarul.cn

[L02] 发送 POST JSON
来源：http://zkm.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ibl.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gne.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bko.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pjv.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lex.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yhs.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wbx.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dyq.vehdjk.com

[L03] 设置自定义请求头
来源：http://aik.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wtf.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vzs.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqy.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdl.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pwh.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bzs.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xny.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ffe.bbcook.cn

[L04] 设置超时
来源：http://sie.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://pwa.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dov.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://znj.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npn.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qhi.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cle.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ueu.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rmm.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://lky.9152youxi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://glk.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rev.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ktj.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qop.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://drf.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://byh.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gxo.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gld.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://vec.guannengcc.top

Py:   resp.json()
来源：http://eey.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://juv.ppjwa.cn

JS:   await resp.json()
来源：http://pmg.gzhubu.top

TS:   await resp.json()
来源：http://una.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nmk.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tlh.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://zuy.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jtd.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://iuu.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://odx.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zvy.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://rcy.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://jxn.birdmap.top

Java: resp.statusCode()
来源：http://nsg.cheryme.top

Go:   resp.StatusCode
来源：http://boa.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://ryp.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://tjw.yfazqb.com

[L08] 并发请求多个地址
来源：http://svk.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://myj.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://xxq.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://upn.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fed.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ruu.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://abu.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nzi.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jta.hesvh.cn

================================================================================
来源：http://fie.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://bqg.xziqi.cn

================================================================================
来源：http://gcb.tanke756.top

[M01] 读取命令行参数
来源：http://zez.sxryk.cn

Py:   sys.argv[1:]
来源：http://gyv.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://cph.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://tmc.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://zxq.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://dnb.hnxiangtu.top

Go:   os.Args[1:]
来源：http://obg.tian-w.cn

Ruby: ARGV
来源：http://khy.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://ycq.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://axt.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://urt.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jpd.ivvv.top

JS:   process.env.HOME
来源：http://fwe.ydjk.org.cn

TS:   process.env.HOME
来源：http://lrc.redwolf501.top

Java: System.getenv("HOME")
来源：http://qeg.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://djo.tanke756.top

Ruby: ENV["HOME"]
来源：http://krf.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iti.bjfxy.top

[M03] 执行外部命令
来源：http://zvb.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fus.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zym.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fte.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://frf.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gem.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rqg.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://dyk.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://pex.dianchejie.cn

[M04] 获取当前工作目录
来源：http://nof.xuanzx.com

Py:   os.getcwd()
来源：http://sls.yongpay.top

PHP:  getcwd();
来源：http://hzh.cqqwz.cn

JS:   process.cwd()
来源：http://vwj.jlsjyb.cn

TS:   process.cwd()
来源：http://djk.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://vjt.zhoulong.xyz

Go:   os.Getwd()
来源：http://lis.jianghu66.top

Ruby: Dir.pwd
来源：http://xmb.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jtw.gotoacloud.top

[M05] 设置退出码
来源：http://azu.sysykeji.top

Py:   sys.exit(1)
来源：http://fqf.pengpengdd.cyou

PHP:  exit(1);
来源：http://zqv.zhijiandao.cn

JS:   process.exit(1)
来源：http://hxq.jqgfzy.top

TS:   process.exit(1)
来源：http://txb.jlsjyb.cn

Java: System.exit(1)
来源：http://mti.yj20258888.top

Go:   os.Exit(1)
来源：http://qzs.sxryk.cn

Ruby: exit 1
来源：http://cwr.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jjt.ivvv.top

[M06] 向标准错误输出
来源：http://ezu.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://muz.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qji.ehwqpu.com

JS:   console.error("err")
来源：http://ana.sweek.top

TS:   console.error("err")
来源：http://pys.shuidangran.top

Java: System.err.println("err")
来源：http://yod.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ofa.chenlongwang.top

Ruby: warn "err"
来源：http://nue.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ltv.dianchejie.cn

[M07] 判断是否为主入口
来源：http://jrk.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://uze.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rvb.svipenyu.cn

JS:   require.main === module
来源：http://yll.shuidangran.top

TS:   require.main === module
来源：http://kbd.hesvh.cn

Java: public static void main(String[] args)
来源：http://zhe.hammf.cn

Go:   func main()
来源：http://jnk.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hhj.yj20258888.top

C#:   static void Main(string[] args)
来源：http://stx.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://trl.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://efv.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://dro.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://ysz.guannengcc.top

TS:   process.platform;  process.version
来源：http://twm.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qru.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tee.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qcn.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pwz.uphjek.com

================================================================================
来源：http://mod.gotoacloud.top

N. 数据结构与算法
来源：http://twf.zhaomingkeji.xyz

================================================================================
来源：http://jol.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://auu.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://oll.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wkx.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxa.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vin.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://cph.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://afc.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://leb.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgc.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://zgv.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://rsh.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ewc.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kpa.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tsa.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wch.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://lnq.yongpay.top

Ruby: arr.sort
来源：http://prr.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsb.yongpay.top

[N03] 快速排序（分治示例）
来源：http://ryz.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tha.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://rpp.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkn.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nrv.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufb.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://med.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dri.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://qaq.jqgfzy.top

[N04] 斐波那契数列
来源：http://hbz.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qxn.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rjm.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upf.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwg.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aze.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iwq.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzj.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://woz.sysykeji.top

[N05] 最大公约数
来源：http://dfg.yonumen.top

Py:   math.gcd(a, b)
来源：http://ohz.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nce.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uef.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzr.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jxf.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lfs.tian-w.cn

Ruby: a.gcd(b)
来源：http://scg.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mep.ctjpmb.com

[N06] 判断回文字符串
来源：http://wnn.jiagoushi.top

Py:   s == s[::-1]
来源：http://rid.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://obs.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://sdd.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://vhu.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blj.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://dge.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ase.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://omf.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://hdh.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bes.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ajo.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zxu.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://uyg.hesvh.cn

Java: // 手写 HashMap
来源：http://bai.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://pju.yj20258.top

Ruby: // 手写 Hash
来源：http://hxp.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://fat.jyoumei.cn

[N08] 生成全排列
来源：http://kdx.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://leb.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://akh.epnwcf.com

JS:   // 手写回溯递归
来源：http://rmr.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://hop.zycfv.cn

Java: // 手写回溯递归
来源：http://zcz.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://phq.uphjek.com

Ruby: arr.permutation.to_a
来源：http://pqd.yangfankeji.com

C#:   // 手写回溯递归
来源：http://iky.jinqigfzy.top

[N09] 栈与队列
来源：http://wbw.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fgg.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ktc.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ihx.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://noe.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bzc.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://igi.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wln.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qpe.sufxvd.cn

[N10] 链表节点定义
来源：http://jtf.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xex.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://lma.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mlu.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xsc.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://gxr.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gkl.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://azd.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fxn.andypj.xyz

[N11] 二叉树中序遍历
来源：http://zop.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rzi.nwbrower.top

PHP:  // 手写递归函数
来源：http://drw.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhj.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdn.ydzc1.top

Java: // 手写递归
来源：http://akw.ehwqpu.com

Go:   // 手写递归
来源：http://ijj.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iim.tian-w.cn

C#:   // 手写递归
来源：http://hma.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ylb.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rtc.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://toa.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhr.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yus.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pyo.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hux.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kpt.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtz.nanxuanxn.top

================================================================================
来源：http://pix.xingfuxueyuan.xyz

O. 并发与异步
来源：http://lkt.gotoacloud.top

================================================================================
来源：http://gff.xinyue.icu

[O01] 启动一个线程
来源：http://wfh.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpb.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pbj.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pyn.xinyue.icu

TS:   // 同 JS
来源：http://rsb.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://jfd.xziqi.cn

Go:   go f()
来源：http://ppe.shuidangran.top

Ruby: Thread.new { f }
来源：http://qmh.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://dqs.shangyingyoupin.top


<!-- 参考信息 -->