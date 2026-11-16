代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://nii.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rdd.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jho.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lyo.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://pne.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lzc.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lpj.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbj.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mze.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hhz.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ktx.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mcd.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vbg.cashguo.top

[K07] 进制转换
来源：http://wew.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vzf.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pgc.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mhn.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tet.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uew.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://drm.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uez.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ggt.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bte.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://dcm.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wzf.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://rmq.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://ffs.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cgl.zhiwuduotai.top

Go:   encoding/gob
来源：http://mel.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://reg.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kls.tian-w.cn

================================================================================
来源：http://mkf.jinqigufen.top

L. 网络请求
来源：http://jnw.zhoulong.xyz

================================================================================
来源：http://uoq.iojbl.cn

[L01] 发送 GET 请求
来源：http://lxg.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xbq.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://thm.zhongyouzk.top

JS:   await fetch(url)
来源：http://ivs.yuxming.cn

TS:   await fetch(url)
来源：http://uug.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iof.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://suk.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vzy.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oek.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://hvj.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bhu.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lhg.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isc.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://beu.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://val.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pop.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqz.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ucz.shuidangran.top

[L03] 设置自定义请求头
来源：http://vhp.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ggv.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://coz.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jzq.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hpj.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://abt.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oen.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rqv.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vqq.guowangkeji.top

[L04] 设置超时
来源：http://dqd.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://jiq.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qbr.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipk.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgj.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yck.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pla.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pqb.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://egm.redwolf501.top

[L05] 上传文件（multipart）
来源：http://qop.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ejx.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tsf.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qbo.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mwa.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmw.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dyv.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vsj.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zqa.bjfxy.top

[L06] 解析响应为 JSON
来源：http://jsm.yangfankeji.com

Py:   resp.json()
来源：http://fvg.hcnkem.com

PHP:  json_decode($body, true);
来源：http://nbg.yfazqb.com

JS:   await resp.json()
来源：http://sof.zhixingplan.top

TS:   await resp.json()
来源：http://jbg.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wrs.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aeb.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://rbv.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjj.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://siy.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gyh.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lwf.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://uuh.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://ckf.zhiwuduotai.top

Java: resp.statusCode()
来源：http://kho.ppjwa.cn

Go:   resp.StatusCode
来源：http://egp.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://rpn.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://uiw.wangdashe.top

[L08] 并发请求多个地址
来源：http://kkc.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dbg.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://qcs.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwa.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwx.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vic.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzx.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zys.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://upr.zhengqikj.top

================================================================================
来源：http://mpr.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://urq.gogol.net.cn

================================================================================
来源：http://uoz.havefunace.top

[M01] 读取命令行参数
来源：http://lni.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://stm.mhx1999.top

PHP:  $argv;  $argc;
来源：http://ntb.shuidangran.top

JS:   process.argv.slice(2)
来源：http://yle.smart0.xyz

TS:   process.argv.slice(2)
来源：http://bjn.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://edx.c1oappe.top

Go:   os.Args[1:]
来源：http://iac.meibo888.top

Ruby: ARGV
来源：http://xxb.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://yvv.tarul.cn

[M02] 读取环境变量
来源：http://ust.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://hmd.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kpd.bbcook.cn

JS:   process.env.HOME
来源：http://oyd.aibaodan.cn

TS:   process.env.HOME
来源：http://tlp.cucudq.cn

Java: System.getenv("HOME")
来源：http://xjr.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ulj.aizwys.cn

Ruby: ENV["HOME"]
来源：http://cdn.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kau.havefunace.top

[M03] 执行外部命令
来源：http://xtn.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://drb.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lnw.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://thq.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ysx.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wcb.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mry.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nfl.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://lkr.cashguo.top

[M04] 获取当前工作目录
来源：http://nsj.daxiang520.top

Py:   os.getcwd()
来源：http://kef.svipenyu.cn

PHP:  getcwd();
来源：http://emw.zhixingplan.top

JS:   process.cwd()
来源：http://qta.jqgufenzy.top

TS:   process.cwd()
来源：http://kku.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://djh.hongshengwenyu.top

Go:   os.Getwd()
来源：http://osk.uphjek.com

Ruby: Dir.pwd
来源：http://dty.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://wbd.cashguo.top

[M05] 设置退出码
来源：http://dap.tarul.cn

Py:   sys.exit(1)
来源：http://qlq.nanxinkj.top

PHP:  exit(1);
来源：http://gat.svipenyu.cn

JS:   process.exit(1)
来源：http://pxx.ydjk.org.cn

TS:   process.exit(1)
来源：http://ohi.vehdjk.com

Java: System.exit(1)
来源：http://rjj.xylfe.cn

Go:   os.Exit(1)
来源：http://axr.yanxiufei.cn

Ruby: exit 1
来源：http://oad.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xkg.ivvv.top

[M06] 向标准错误输出
来源：http://wle.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://hds.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://jvc.wangdashe.top

JS:   console.error("err")
来源：http://efc.shanyushiyangtech.top

TS:   console.error("err")
来源：http://wyc.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://yei.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pmw.hywenlv.cn

Ruby: warn "err"
来源：http://jct.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://bbx.fengsongda.top

[M07] 判断是否为主入口
来源：http://hba.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://vvo.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zgm.gogol.net.cn

JS:   require.main === module
来源：http://mrj.c1oappe.top

TS:   require.main === module
来源：http://fay.xuanzx.com

Java: public static void main(String[] args)
来源：http://cap.tian-w.cn

Go:   func main()
来源：http://yty.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yoy.yuxming.cn

C#:   static void Main(string[] args)
来源：http://zrl.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://caa.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://euh.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://ecl.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://vlc.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://tir.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qnj.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fve.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://opp.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mji.yvedp.cn

================================================================================
来源：http://pfz.ydjk.org.cn

N. 数据结构与算法
来源：http://hqs.zhijiandao.cn

================================================================================
来源：http://gsk.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://cuo.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://qmg.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://chh.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wxz.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfq.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://dmj.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://txf.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wma.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://bwd.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://hue.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://abg.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wjc.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://yeo.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://glh.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://voq.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://fbw.pengpengdd.cyou

Ruby: arr.sort
来源：http://yzo.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gep.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://wlb.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wke.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://wxk.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hae.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qka.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pbf.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hku.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://prp.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://qtp.jqgufenzy.top

[N04] 斐波那契数列
来源：http://hxd.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://imn.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hhc.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bza.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rxe.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bya.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sps.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lcq.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wwm.guannengcc.top

[N05] 最大公约数
来源：http://xin.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://enx.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qyb.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynp.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tyv.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hou.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lcy.ydzc1.top

Ruby: a.gcd(b)
来源：http://lxj.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kwy.ydzc1.top

[N06] 判断回文字符串
来源：http://hrx.hnqzz.top

Py:   s == s[::-1]
来源：http://dsl.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://lzh.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://dvk.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://mbh.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rlw.shuidangran.top

Go:   // 双指针从两端比较
来源：http://gtt.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://bdl.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hap.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://goz.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pha.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jcm.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eil.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://nln.birdmap.top

Java: // 手写 HashMap
来源：http://cdh.yj202588.top

Go:   // 手写 map[int]int
来源：http://zrm.xylfe.cn

Ruby: // 手写 Hash
来源：http://yfv.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://zhh.ydjk.org.cn

[N08] 生成全排列
来源：http://hfj.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://pya.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://abp.zhengqikj.top

JS:   // 手写回溯递归
来源：http://gdv.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://klj.yj20258888.top

Java: // 手写回溯递归
来源：http://drf.smart0.xyz

Go:   // 手写回溯递归
来源：http://ayj.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://ita.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://cys.pycfn.com

[N09] 栈与队列
来源：http://gyn.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dxb.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bfq.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hbx.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://glp.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dka.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pfw.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pji.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxy.pycfn.com

[N10] 链表节点定义
来源：http://xie.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mwv.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zzw.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zdj.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vuu.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://csn.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aoh.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://puk.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mah.cashguo.top

[N11] 二叉树中序遍历
来源：http://kox.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://opc.ybcxt.top

PHP:  // 手写递归函数
来源：http://lzy.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vzh.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmz.tanke756.top

Java: // 手写递归
来源：http://yjv.jlsjyb.cn

Go:   // 手写递归
来源：http://ydu.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wxw.andypj.xyz

C#:   // 手写递归
来源：http://gmt.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qxa.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opm.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fhz.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yly.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kon.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://egu.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zla.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcy.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://drg.vqdsnc.cn

================================================================================
来源：http://mks.fanxiaobao.xyz

O. 并发与异步
来源：http://afn.shanyushiyangtech.top

================================================================================
来源：http://lmg.jianghu66.top

[O01] 启动一个线程
来源：http://xvj.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dyd.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fde.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xbv.tarul.cn

TS:   // 同 JS
来源：http://kai.tianlin.xyz


<!-- 参考信息 -->