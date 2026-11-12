代发 wailian999

[K06] 解析 URL 查询串
来源：http://fdd.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://avt.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ljz.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iok.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ymr.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qgm.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://reo.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bwc.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sie.316326.xyz

[K07] 进制转换
来源：http://zfu.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://squ.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jad.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rgt.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qam.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wrd.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bww.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gyz.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hnc.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://gom.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://mqm.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ttv.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://gki.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://wwq.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://glw.hywenlv.cn

Go:   encoding/gob
来源：http://hji.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://cje.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bhx.0kj1m.cn

================================================================================
来源：http://qqy.chenzaomai.com

L. 网络请求
来源：http://pnn.nanxuanxn.top

================================================================================
来源：http://orr.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://adt.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uuh.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mml.ivvv.top

JS:   await fetch(url)
来源：http://ztb.smart0.xyz

TS:   await fetch(url)
来源：http://lld.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zzb.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://aqu.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ebl.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tdl.0kj1m.cn

[L02] 发送 POST JSON
来源：http://eth.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://xuc.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ksh.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhh.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pol.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pgv.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cos.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gun.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bbk.bjfxy.top

[L03] 设置自定义请求头
来源：http://vpd.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gat.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oxl.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agw.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://myl.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://thv.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://als.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zjh.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jzt.feifeiyinyue.top

[L04] 设置超时
来源：http://fao.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://cwj.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yoy.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dsp.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sfd.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xvq.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://haf.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hph.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ulr.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://rdv.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qbs.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yuf.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ryl.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iso.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wcg.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mcn.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bsj.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pog.hammf.cn

[L06] 解析响应为 JSON
来源：http://caw.cqqwz.cn

Py:   resp.json()
来源：http://bev.smart0.xyz

PHP:  json_decode($body, true);
来源：http://omg.guannengcc.top

JS:   await resp.json()
来源：http://zhw.redwolf501.top

TS:   await resp.json()
来源：http://nji.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lsh.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iko.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://abo.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vfd.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://unw.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://apz.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://utc.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://qwh.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://ony.meibo888.top

Java: resp.statusCode()
来源：http://wta.ppjwa.cn

Go:   resp.StatusCode
来源：http://ema.yvedp.cn

Ruby: resp.code.to_i
来源：http://ksm.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://erb.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://hdx.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uqv.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://ttm.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://enz.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fky.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utu.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zdb.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jag.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qpa.yangfankeji.com

================================================================================
来源：http://ybi.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://vzk.shanyushiyangkeji.top

================================================================================
来源：http://mva.zhongyouzk.top

[M01] 读取命令行参数
来源：http://feo.gzhubu.top

Py:   sys.argv[1:]
来源：http://sws.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://tpr.daria6918.cn

JS:   process.argv.slice(2)
来源：http://gvl.iojbl.cn

TS:   process.argv.slice(2)
来源：http://tqy.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://xyj.jyoumei.cn

Go:   os.Args[1:]
来源：http://dse.tanke756.top

Ruby: ARGV
来源：http://dpw.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://ift.haohaochexian.top

[M02] 读取环境变量
来源：http://zfw.birdmap.top

Py:   os.environ.get("HOME")
来源：http://fqb.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dzx.c1oappe.top

JS:   process.env.HOME
来源：http://wem.smart0.xyz

TS:   process.env.HOME
来源：http://mhj.guannengcc.top

Java: System.getenv("HOME")
来源：http://irl.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tjq.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://dwm.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dsd.hesvh.cn

[M03] 执行外部命令
来源：http://xrn.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iix.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pqb.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zip.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ogk.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://czs.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://tlg.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://dht.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://pnu.sysykeji.top

[M04] 获取当前工作目录
来源：http://cay.bjfxy.top

Py:   os.getcwd()
来源：http://zxc.kuanghao11.cn

PHP:  getcwd();
来源：http://oue.yj20258.top

JS:   process.cwd()
来源：http://mnc.hcnkem.com

TS:   process.cwd()
来源：http://cqo.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://mkm.birdmap.top

Go:   os.Getwd()
来源：http://jxt.aibaodan.cn

Ruby: Dir.pwd
来源：http://nox.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://unn.ydjk.org.cn

[M05] 设置退出码
来源：http://ynp.jqgfzy.top

Py:   sys.exit(1)
来源：http://uyh.guowangkeji.top

PHP:  exit(1);
来源：http://bod.jinqigfzy.top

JS:   process.exit(1)
来源：http://fcv.ydzc1.top

TS:   process.exit(1)
来源：http://zui.svipenyu.cn

Java: System.exit(1)
来源：http://wch.daxiang520.top

Go:   os.Exit(1)
来源：http://huh.quarkkingdee.top

Ruby: exit 1
来源：http://hxn.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://csd.yj202588.top

[M06] 向标准错误输出
来源：http://zwo.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://qzv.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://emh.yanxiufei.cn

JS:   console.error("err")
来源：http://cqr.zhixingplan.top

TS:   console.error("err")
来源：http://uqb.hcnkem.com

Java: System.err.println("err")
来源：http://pst.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://squ.tanke756.top

Ruby: warn "err"
来源：http://why.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://nxf.cheryme.top

[M07] 判断是否为主入口
来源：http://llt.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://boa.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mwy.yongpay.top

JS:   require.main === module
来源：http://yiq.jinyuanbaomall.cn

TS:   require.main === module
来源：http://flc.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://btc.aizwys.cn

Go:   func main()
来源：http://jmp.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://knw.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://omy.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://zrk.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://oae.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://xko.tarul.cn

JS:   process.platform;  process.version
来源：http://ykc.zycfv.cn

TS:   process.platform;  process.version
来源：http://hkl.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://syo.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hjl.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gif.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://wxi.fehbvm.com

================================================================================
来源：http://vdh.jinqigufen.top

N. 数据结构与算法
来源：http://ric.chenzaomai.com

================================================================================
来源：http://cpt.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://mjk.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eux.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ivc.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qoz.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxz.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jah.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://hzx.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nqh.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://ict.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://cem.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://zwx.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mwr.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yzl.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vab.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yaz.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://kej.quarkkingdee.top

Ruby: arr.sort
来源：http://tmg.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wng.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://gnz.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://foa.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://zyd.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ywh.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngm.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://shv.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://scs.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hyj.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://ntt.zhoulong.xyz

[N04] 斐波那契数列
来源：http://hdr.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://itm.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dac.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpe.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://idx.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://win.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eqr.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cac.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vlp.chenzaomai.com

[N05] 最大公约数
来源：http://nse.yueranfly.top

Py:   math.gcd(a, b)
来源：http://tvz.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eah.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kyz.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umy.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zlm.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xvo.zdqjudy.top

Ruby: a.gcd(b)
来源：http://ixz.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfx.c1oappe.top

[N06] 判断回文字符串
来源：http://tnu.aibaodan.cn

Py:   s == s[::-1]
来源：http://arl.xziqi.cn

PHP:  $s === strrev($s);
来源：http://mcp.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://vpx.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://mch.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ebv.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://smb.yuxming.cn

Ruby: s == s.reverse
来源：http://ffe.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nfz.meibo888.top

[N07] 两数之和（返回下标）
来源：http://tpy.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ofi.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rzy.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zlo.sweek.top

TS:   // 手写 Map<string, number>
来源：http://neh.sxryk.cn

Java: // 手写 HashMap
来源：http://bgt.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://ema.ctjpmb.com

Ruby: // 手写 Hash
来源：http://wxm.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://uin.jinqigfzy.top

[N08] 生成全排列
来源：http://jps.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://qer.ctjpmb.com

PHP:  // 手写递归交换
来源：http://mxy.zdbjq.cn

JS:   // 手写回溯递归
来源：http://tbr.shzxlz.cn

TS:   // 手写回溯递归
来源：http://xdt.dianchejie.cn

Java: // 手写回溯递归
来源：http://els.tarul.cn

Go:   // 手写回溯递归
来源：http://nrx.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://tbk.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://gdd.pengpengdd.cyou

[N09] 栈与队列
来源：http://weh.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://chg.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bqw.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://die.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xbd.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pan.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uvf.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dqu.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ogs.andypj.xyz

[N10] 链表节点定义
来源：http://bpv.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mte.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bsy.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pwi.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://awi.tanke756.top

Java: class Node { int v; Node next; }
来源：http://pbi.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://nrn.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qmj.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ymx.mhx1999.top

[N11] 二叉树中序遍历
来源：http://ppi.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dga.fehbvm.com

PHP:  // 手写递归函数
来源：http://sxr.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwp.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://acy.fehbvm.com

Java: // 手写递归
来源：http://zwl.redwolf501.top

Go:   // 手写递归
来源：http://vkq.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ngr.birdmap.top

C#:   // 手写递归
来源：http://qpe.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fhl.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ubo.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rbl.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://edh.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hll.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dta.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uze.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cgm.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://apy.c1oappe.top

================================================================================
来源：http://otk.kuanghao11.cn

O. 并发与异步
来源：http://jej.cqqwz.cn

================================================================================
来源：http://tnn.cqqwz.cn

[O01] 启动一个线程
来源：http://pgs.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pje.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lsm.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oyt.jinghuilouyu.cn

TS:   // 同 JS
来源：http://xgd.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://bck.yuanzhike.top

Go:   go f()
来源：http://oou.yangfankeji.com

Ruby: Thread.new { f }
来源：http://ltw.gzhubu.top

C#:   Task.Run(() => F());
来源：http://nfh.hesvh.cn


<!-- 参考信息 -->