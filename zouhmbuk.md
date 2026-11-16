代发 wailian999

[K06] 解析 URL 查询串
来源：http://apl.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eux.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ytl.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ydb.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bam.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pne.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wao.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://llt.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lri.mhx1999.top

[K07] 进制转换
来源：http://fgu.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bhr.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jti.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vfn.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://doq.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zyg.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kej.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mjd.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://klm.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://pii.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://mes.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nph.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://nns.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://rsr.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://abc.jinqigfzy.top

Go:   encoding/gob
来源：http://ivo.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://tab.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yvd.shanyushiyangkeji.top

================================================================================
来源：http://rdi.chenjidiqi.icu

L. 网络请求
来源：http://mpw.jinghuilouyu.cn

================================================================================
来源：http://flg.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://cun.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uey.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iyj.sysykeji.top

JS:   await fetch(url)
来源：http://wpl.zhengqikj.top

TS:   await fetch(url)
来源：http://gsw.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kmn.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://mmo.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gfj.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgd.cucudq.cn

[L02] 发送 POST JSON
来源：http://jcy.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://tej.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xes.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xgw.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aii.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iqu.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hxo.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qqh.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://knn.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://haf.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://guf.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xyb.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlw.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://stc.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avx.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://glw.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qde.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://npr.fzhhl.top

[L04] 设置超时
来源：http://emh.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://trf.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://irg.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rae.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfo.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://btg.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uud.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bwc.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fjs.gzhubu.top

[L05] 上传文件（multipart）
来源：http://zau.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wto.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ptz.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wtm.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fzw.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ojy.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dtt.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vkr.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pus.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://wpn.bbcook.cn

Py:   resp.json()
来源：http://noa.yvedp.cn

PHP:  json_decode($body, true);
来源：http://elq.wangshuangyany.cn

JS:   await resp.json()
来源：http://itx.zhiwuduotai.top

TS:   await resp.json()
来源：http://unv.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bzt.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://loh.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://jwr.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cwl.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://cgx.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lwn.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mgp.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://byt.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://uqo.wangshuangyany.cn

Java: resp.statusCode()
来源：http://zhf.fzhhl.top

Go:   resp.StatusCode
来源：http://xkb.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://fyn.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://ydg.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://kqy.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hjs.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://lrt.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwb.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwm.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://svl.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lmc.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://abe.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://auv.epnwcf.com

================================================================================
来源：http://qhh.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://qio.shanyushiyangkeji.top

================================================================================
来源：http://zjc.ppjwa.cn

[M01] 读取命令行参数
来源：http://bfs.yuanzhike.top

Py:   sys.argv[1:]
来源：http://ofy.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://wkx.fengsongda.top

JS:   process.argv.slice(2)
来源：http://fur.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://aoz.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://gzj.yueranfly.top

Go:   os.Args[1:]
来源：http://uta.ivvv.top

Ruby: ARGV
来源：http://vqx.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://wtq.uphjek.com

[M02] 读取环境变量
来源：http://wvn.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://eeh.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hej.zhengqikj.top

JS:   process.env.HOME
来源：http://tyl.yvedp.cn

TS:   process.env.HOME
来源：http://pih.yj202588.top

Java: System.getenv("HOME")
来源：http://suq.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://arj.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://uxh.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sgi.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://hvh.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wfq.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lhw.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://egq.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bfw.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ggo.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wiq.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://atp.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://nyt.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://alz.gaohongyu789.top

Py:   os.getcwd()
来源：http://mio.haohaochexian.top

PHP:  getcwd();
来源：http://tzw.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://wdy.cqqwz.cn

TS:   process.cwd()
来源：http://mfe.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://yac.zdbjq.cn

Go:   os.Getwd()
来源：http://ejo.jinqigfzy.top

Ruby: Dir.pwd
来源：http://lso.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mxd.vehdjk.com

[M05] 设置退出码
来源：http://gzq.ppjwa.cn

Py:   sys.exit(1)
来源：http://ihc.fanxiaobao.xyz

PHP:  exit(1);
来源：http://bac.tanke756.top

JS:   process.exit(1)
来源：http://nmx.c1oappe.top

TS:   process.exit(1)
来源：http://ubj.sufxvd.cn

Java: System.exit(1)
来源：http://aep.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://thk.hcnkem.com

Ruby: exit 1
来源：http://cmc.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ktk.hammf.cn

[M06] 向标准错误输出
来源：http://wel.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://xzu.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xyc.yueranfly.top

JS:   console.error("err")
来源：http://vny.hammf.cn

TS:   console.error("err")
来源：http://blk.sysykeji.top

Java: System.err.println("err")
来源：http://lso.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xnz.andypj.xyz

Ruby: warn "err"
来源：http://gke.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://uhs.zycfv.cn

[M07] 判断是否为主入口
来源：http://nbo.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://sfy.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://epx.9152youxi.cn

JS:   require.main === module
来源：http://kqa.yongpay.top

TS:   require.main === module
来源：http://zwo.fktsv.cn

Java: public static void main(String[] args)
来源：http://btc.iojbl.cn

Go:   func main()
来源：http://nax.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wpn.cucudq.cn

C#:   static void Main(string[] args)
来源：http://qem.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://cib.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://bxf.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://udd.nanxinkj.top

JS:   process.platform;  process.version
来源：http://lap.daria6918.cn

TS:   process.platform;  process.version
来源：http://nrk.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rzr.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xxt.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rbi.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vgu.redwolf501.top

================================================================================
来源：http://eot.sjlbkw.cn

N. 数据结构与算法
来源：http://fjv.kuanghao11.cn

================================================================================
来源：http://zck.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://bhn.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jto.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kfw.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmy.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eoi.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gxi.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ghz.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mcj.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sdi.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://zxd.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://lkw.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bll.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlw.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mvl.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://owm.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://vxu.vqdsnc.cn

Ruby: arr.sort
来源：http://sxx.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hvv.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://gup.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ilb.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://udf.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ily.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nve.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uny.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dki.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nsg.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oze.hammf.cn

[N04] 斐波那契数列
来源：http://sxs.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jcl.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fhf.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://giw.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lnq.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vuo.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pqz.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nmu.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wkm.iojbl.cn

[N05] 最大公约数
来源：http://tow.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://ixa.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zbg.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://syr.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjl.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mdy.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vmr.tanke756.top

Ruby: a.gcd(b)
来源：http://dep.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rtx.sweek.top

[N06] 判断回文字符串
来源：http://fvl.smart0.xyz

Py:   s == s[::-1]
来源：http://kes.nwbrower.top

PHP:  $s === strrev($s);
来源：http://oof.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://rct.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://dnw.yj20258.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kaf.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://qls.aizwys.cn

Ruby: s == s.reverse
来源：http://osw.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dwl.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://txy.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jfr.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://efx.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kca.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://vnr.hywenlv.cn

Java: // 手写 HashMap
来源：http://zqq.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://fxp.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://yev.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://kpe.yongpay.top

[N08] 生成全排列
来源：http://zna.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://ysr.nwbrower.top

PHP:  // 手写递归交换
来源：http://mie.gogol.net.cn

JS:   // 手写回溯递归
来源：http://xbm.iojbl.cn

TS:   // 手写回溯递归
来源：http://dgj.hammf.cn

Java: // 手写回溯递归
来源：http://rkb.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://sqg.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://ect.yj20258.top

C#:   // 手写回溯递归
来源：http://qru.gogol.net.cn

[N09] 栈与队列
来源：http://axm.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lyu.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nof.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://grb.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fjc.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fpy.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fnf.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eqg.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sns.yuanzhike.top

[N10] 链表节点定义
来源：http://foc.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kme.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://tmc.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zsu.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://edf.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://ias.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://oca.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wwv.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fsg.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://xvi.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vpm.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://hzj.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yby.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsn.zhijiandao.cn

Java: // 手写递归
来源：http://bfx.haohaochexian.top

Go:   // 手写递归
来源：http://iwh.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cuq.xziqi.cn

C#:   // 手写递归
来源：http://npv.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ftb.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szl.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zgr.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jrg.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnl.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ywv.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rvq.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jeg.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ifg.hywenlv.cn

================================================================================
来源：http://xej.haohaochexian.top

O. 并发与异步
来源：http://xto.xziqi.cn

================================================================================
来源：http://jbk.sxryk.cn

[O01] 启动一个线程
来源：http://jdh.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hpe.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eps.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpr.hfpthk.cn

TS:   // 同 JS
来源：http://tox.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://wav.xuanzx.com

Go:   go f()
来源：http://opr.ivvv.top

Ruby: Thread.new { f }
来源：http://gcr.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://umm.fzhhl.top


<!-- 参考信息 -->