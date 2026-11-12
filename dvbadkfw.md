代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hiw.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fzx.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bfc.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mev.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lcb.tian-w.cn

[K07] 进制转换
来源：http://din.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rvx.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zwr.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zfx.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nsg.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tlp.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://huc.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nxt.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gvd.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://yxq.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://col.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vmj.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://car.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://vit.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dof.hnxiangtu.top

Go:   encoding/gob
来源：http://scl.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://zls.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://des.hesvh.cn

================================================================================
来源：http://jqd.ydzc1.top

L. 网络请求
来源：http://ica.0kj1m.cn

================================================================================
来源：http://dny.yuxming.cn

[L01] 发送 GET 请求
来源：http://fka.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://czl.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ckp.hcnkem.com

JS:   await fetch(url)
来源：http://azi.shangyingyoupin.top

TS:   await fetch(url)
来源：http://fij.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hwk.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://ufz.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pdl.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vni.sysykeji.top

[L02] 发送 POST JSON
来源：http://hhc.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://sab.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fqu.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkb.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvt.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bxz.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://snq.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xif.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kpk.wangdashe.top

[L03] 设置自定义请求头
来源：http://szt.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfy.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://evx.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycd.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qca.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xwc.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pxt.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://srr.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vvi.gotoacloud.top

[L04] 设置超时
来源：http://mus.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://xgl.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zrs.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fss.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyi.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qds.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dre.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bmk.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cej.hammf.cn

[L05] 上传文件（multipart）
来源：http://jhn.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://txq.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://itv.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnc.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://coi.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nsn.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uiv.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fxm.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dne.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://osn.ybcxt.top

Py:   resp.json()
来源：http://nyr.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://cer.shanyushiyangtech.top

JS:   await resp.json()
来源：http://iah.guannengcc.top

TS:   await resp.json()
来源：http://bhb.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dae.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bqk.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://bdd.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nfk.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://wec.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nym.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hie.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://ftv.ivvv.top

TS:   resp.ok;  resp.status
来源：http://qyr.shuidangran.top

Java: resp.statusCode()
来源：http://ity.havefunace.top

Go:   resp.StatusCode
来源：http://vvi.jyoumei.cn

Ruby: resp.code.to_i
来源：http://dyt.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://hca.gzhubu.top

[L08] 并发请求多个地址
来源：http://aju.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://udh.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://uow.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pmf.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xia.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://twx.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yqh.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cey.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xuh.yangfankeji.com

================================================================================
来源：http://xpk.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://cxn.jyoumei.cn

================================================================================
来源：http://jdr.pycfn.com

[M01] 读取命令行参数
来源：http://rxd.yj20258888.top

Py:   sys.argv[1:]
来源：http://zwi.cucudq.cn

PHP:  $argv;  $argc;
来源：http://ign.guannengcc.top

JS:   process.argv.slice(2)
来源：http://yhh.nwbrower.top

TS:   process.argv.slice(2)
来源：http://tqy.yj202588.top

Java: args 数组（main 方法参数）
来源：http://tfl.vqdsnc.cn

Go:   os.Args[1:]
来源：http://vyc.daxiang520.top

Ruby: ARGV
来源：http://zht.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://yli.nanxuanxn.top

[M02] 读取环境变量
来源：http://ull.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://blo.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uqe.ctjpmb.com

JS:   process.env.HOME
来源：http://gqf.jinqigfzy.top

TS:   process.env.HOME
来源：http://gly.hfpthk.cn

Java: System.getenv("HOME")
来源：http://gxu.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tvj.birdmap.top

Ruby: ENV["HOME"]
来源：http://kfo.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xwe.zhiwuduotai.top

[M03] 执行外部命令
来源：http://hky.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vwi.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://enj.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jnj.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uoo.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://skq.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cjw.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fjl.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://hdq.tarul.cn

[M04] 获取当前工作目录
来源：http://kfr.yfazqb.com

Py:   os.getcwd()
来源：http://uer.chenlongwang.top

PHP:  getcwd();
来源：http://ein.svipenyu.cn

JS:   process.cwd()
来源：http://rdz.svipenyu.cn

TS:   process.cwd()
来源：http://str.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://ywe.daria6918.cn

Go:   os.Getwd()
来源：http://pus.zdbjq.cn

Ruby: Dir.pwd
来源：http://buc.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ugl.cucudq.cn

[M05] 设置退出码
来源：http://efx.quarkkingdee.top

Py:   sys.exit(1)
来源：http://xmh.jyoumei.cn

PHP:  exit(1);
来源：http://veb.tianlin.xyz

JS:   process.exit(1)
来源：http://rzt.sysykeji.top

TS:   process.exit(1)
来源：http://xdv.nanxuanxn.top

Java: System.exit(1)
来源：http://zyq.yongpay.top

Go:   os.Exit(1)
来源：http://cio.nwbrower.top

Ruby: exit 1
来源：http://vif.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bqz.ybcxt.top

[M06] 向标准错误输出
来源：http://dnb.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://upt.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xqi.fzhhl.top

JS:   console.error("err")
来源：http://nix.hnxiangtu.top

TS:   console.error("err")
来源：http://eny.redwolf501.top

Java: System.err.println("err")
来源：http://tyj.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mdm.daria6918.cn

Ruby: warn "err"
来源：http://gkf.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://ece.haohaochexian.top

[M07] 判断是否为主入口
来源：http://fgr.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://cec.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pxc.pycfn.com

JS:   require.main === module
来源：http://wlt.bjfxy.top

TS:   require.main === module
来源：http://nno.nanxuanxn.top

Java: public static void main(String[] args)
来源：http://fcc.jinyuanbaomall.cn

Go:   func main()
来源：http://gnx.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mjr.zycfv.cn

C#:   static void Main(string[] args)
来源：http://sos.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://bmh.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://hfv.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://beg.yuanzhike.top

JS:   process.platform;  process.version
来源：http://alv.bbcook.cn

TS:   process.platform;  process.version
来源：http://sdd.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wgq.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sqm.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://piz.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://iga.xziqi.cn

================================================================================
来源：http://dxu.nwbrower.top

N. 数据结构与算法
来源：http://pqb.wangshuangyany.cn

================================================================================
来源：http://dsv.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://avf.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pmg.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yxo.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfy.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djc.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://mjg.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://bqu.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hjb.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kqk.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://cit.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://kuu.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lwf.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://awi.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sxm.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wlc.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://daj.jqgufenzy.top

Ruby: arr.sort
来源：http://vki.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pab.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://veo.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ykf.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://zxm.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngr.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnr.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fwo.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oyh.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vjs.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://qgu.yonumen.top

[N04] 斐波那契数列
来源：http://ldf.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dzf.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oqc.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://anx.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdo.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pkc.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wuz.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lwc.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pni.hcnkem.com

[N05] 最大公约数
来源：http://wyn.gzhubu.top

Py:   math.gcd(a, b)
来源：http://puh.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lti.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oii.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uan.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://keq.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zin.cdnleiting.top

Ruby: a.gcd(b)
来源：http://zfq.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qfx.hesvh.cn

[N06] 判断回文字符串
来源：http://nhv.guannengcc.top

Py:   s == s[::-1]
来源：http://jve.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://lqu.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://ktb.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://lku.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tmc.hammf.cn

Go:   // 双指针从两端比较
来源：http://uvn.ctjpmb.com

Ruby: s == s.reverse
来源：http://gmp.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bma.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://toa.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zgu.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lkf.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qna.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://cjx.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://vld.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://lkk.cdnleiting.top

Ruby: // 手写 Hash
来源：http://rqw.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://fmb.tanke756.top

[N08] 生成全排列
来源：http://swg.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://ciu.cashguo.top

PHP:  // 手写递归交换
来源：http://eit.sufxvd.cn

JS:   // 手写回溯递归
来源：http://mhd.fengsongda.top

TS:   // 手写回溯递归
来源：http://grm.yuxming.cn

Java: // 手写回溯递归
来源：http://kzp.shuidangran.top

Go:   // 手写回溯递归
来源：http://vnf.yj202588.top

Ruby: arr.permutation.to_a
来源：http://flu.chenlongwang.top

C#:   // 手写回溯递归
来源：http://lmu.pycfn.com

[N09] 栈与队列
来源：http://mmf.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qae.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uvp.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wts.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bcx.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fgj.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kcv.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jan.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ecd.zhijiandao.cn

[N10] 链表节点定义
来源：http://nso.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ijp.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xco.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kwj.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdi.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://ytb.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://kdx.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://moh.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mcn.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://emm.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lav.redwolf501.top

PHP:  // 手写递归函数
来源：http://bwl.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xnc.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uic.zhaomingkeji.xyz

Java: // 手写递归
来源：http://ywf.zdbjq.cn

Go:   // 手写递归
来源：http://qpi.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cmw.dianchejie.cn

C#:   // 手写递归
来源：http://kit.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kqa.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://igf.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://scr.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://csm.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jjk.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gum.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kah.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sfv.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fss.birdmap.top

================================================================================
来源：http://qkc.yangfankeji.com

O. 并发与异步
来源：http://vlo.dianchejie.cn

================================================================================
来源：http://cad.ehwqpu.com

[O01] 启动一个线程
来源：http://duu.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uwp.iojbl.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://imz.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://brt.feifeiyinyue.top

TS:   // 同 JS
来源：http://qxm.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://bja.gogol.net.cn

Go:   go f()
来源：http://npz.sysykeji.top

Ruby: Thread.new { f }
来源：http://yrs.nwbrower.top

C#:   Task.Run(() => F());
来源：http://hbk.cdnleiting.top

[O02] 使用线程池
来源：http://gvx.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jkk.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ikz.nwbrower.top

JS:   // worker_threads 线程池
来源：http://isc.hnqzz.top


<!-- 参考信息 -->