代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://rxp.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://opa.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://sis.fktsv.cn

TS:   structuredClone(obj)
来源：http://pye.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tqp.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kww.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kkm.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jdv.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://pqf.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lzi.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tbn.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blt.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hla.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jdk.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rzc.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yuq.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tag.yj202588.top

[K07] 进制转换
来源：http://yel.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qpj.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yts.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tkv.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cti.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ilr.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vak.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oge.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hvs.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://dyv.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://zme.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ixy.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://krf.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://xnx.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yqn.gaohongyu789.top

Go:   encoding/gob
来源：http://mbq.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://tjb.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://whq.shuidangran.top

================================================================================
来源：http://mgp.shangyingyoupin.top

L. 网络请求
来源：http://ezy.ywan-chungtsiang.top

================================================================================
来源：http://ary.hcnkem.com

[L01] 发送 GET 请求
来源：http://olv.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bui.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://luy.gaohongyu789.top

JS:   await fetch(url)
来源：http://com.hywenlv.cn

TS:   await fetch(url)
来源：http://hyg.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mem.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://rsx.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yop.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kky.fehbvm.com

[L02] 发送 POST JSON
来源：http://ucu.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://lxb.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ywo.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://toq.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bcf.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vky.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vey.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://euu.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ram.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://kec.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dsp.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xra.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgx.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://anz.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rcq.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://anr.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://prx.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wuw.dashuyun.cn

[L04] 设置超时
来源：http://ijy.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://ylz.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qzt.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gvj.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hjz.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bfo.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gdh.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nps.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lxx.sxryk.cn

[L05] 上传文件（multipart）
来源：http://goy.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dln.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mma.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nag.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dvx.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ist.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zfa.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://alz.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://txs.tanke756.top

[L06] 解析响应为 JSON
来源：http://ljn.hammf.cn

Py:   resp.json()
来源：http://emz.52xcode.cn

PHP:  json_decode($body, true);
来源：http://xdg.shangyingyoupin.top

JS:   await resp.json()
来源：http://rsi.bjfxy.top

TS:   await resp.json()
来源：http://fic.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hao.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sur.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://ipc.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pbq.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://hcn.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ddc.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iyn.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://ygg.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://ntk.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://gcx.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://nvx.cucudq.cn

Ruby: resp.code.to_i
来源：http://dwa.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://hyg.shuidangran.top

[L08] 并发请求多个地址
来源：http://wcx.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://szi.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://auq.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wzm.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://icm.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sed.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vbx.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://plg.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qib.wangdashe.top

================================================================================
来源：http://wlc.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://mfe.xziqi.cn

================================================================================
来源：http://pdt.nanxinkj.top

[M01] 读取命令行参数
来源：http://qad.dianchejie.cn

Py:   sys.argv[1:]
来源：http://unp.yj20258.top

PHP:  $argv;  $argc;
来源：http://ppe.havefunace.top

JS:   process.argv.slice(2)
来源：http://zdd.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://xms.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://clj.yongpay.top

Go:   os.Args[1:]
来源：http://qcx.zhongyouzk.top

Ruby: ARGV
来源：http://qaw.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://pnz.hywenlv.cn

[M02] 读取环境变量
来源：http://thu.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://srk.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bvl.daria6918.cn

JS:   process.env.HOME
来源：http://zak.chenjidiqi.icu

TS:   process.env.HOME
来源：http://spc.gzhubu.top

Java: System.getenv("HOME")
来源：http://usa.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgk.yfazqb.com

Ruby: ENV["HOME"]
来源：http://bli.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://djk.bjfxy.top

[M03] 执行外部命令
来源：http://tqk.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://whb.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kmk.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cfc.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wpj.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://glz.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vau.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ekr.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://ppr.chenzaomai.com

[M04] 获取当前工作目录
来源：http://qbr.cheryme.top

Py:   os.getcwd()
来源：http://asn.zhiwuduotai.top

PHP:  getcwd();
来源：http://vgb.0kj1m.cn

JS:   process.cwd()
来源：http://hzh.hfpthk.cn

TS:   process.cwd()
来源：http://cfn.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://nou.zhiwuduotai.top

Go:   os.Getwd()
来源：http://kty.zhengqikj.top

Ruby: Dir.pwd
来源：http://fuv.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://ssa.wangshuangyany.cn

[M05] 设置退出码
来源：http://clz.cheryme.top

Py:   sys.exit(1)
来源：http://pax.cdnleiting.top

PHP:  exit(1);
来源：http://lvr.chenjidiqi.icu

JS:   process.exit(1)
来源：http://slf.fehbvm.com

TS:   process.exit(1)
来源：http://ubl.tarul.cn

Java: System.exit(1)
来源：http://sin.hysaishi.cn

Go:   os.Exit(1)
来源：http://ieh.hammf.cn

Ruby: exit 1
来源：http://mjy.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://btk.hywenlv.cn

[M06] 向标准错误输出
来源：http://ikc.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://nrb.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aje.meibo888.top

JS:   console.error("err")
来源：http://kya.jianghu66.top

TS:   console.error("err")
来源：http://mjs.cheryme.top

Java: System.err.println("err")
来源：http://agz.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://leu.shuidangran.top

Ruby: warn "err"
来源：http://hhw.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://gjg.ivvv.top

[M07] 判断是否为主入口
来源：http://okq.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://hma.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqy.yj20258.top

JS:   require.main === module
来源：http://cof.kuanghao11.cn

TS:   require.main === module
来源：http://xmb.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://gek.gzhubu.top

Go:   func main()
来源：http://wsr.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qlc.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://ntt.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://bna.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://aes.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://duc.yuanzhike.top

JS:   process.platform;  process.version
来源：http://aeq.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://uej.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aix.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ztz.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xon.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eub.yuanzhike.top

================================================================================
来源：http://fxa.bjfxy.top

N. 数据结构与算法
来源：http://nvk.ybcxt.top

================================================================================
来源：http://sny.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://ojq.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://vqq.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sta.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://evh.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://evn.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lql.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://tvr.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://whc.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://lcu.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://wcn.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://vcq.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://noi.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bqn.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lkd.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oom.fengsongda.top

Go:   slices.Sort(arr)
来源：http://vxk.quarkkingdee.top

Ruby: arr.sort
来源：http://thu.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybo.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://uyg.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://djc.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://dwu.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axg.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hei.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kzx.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qvj.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://quh.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://cnc.haohaochexian.top

[N04] 斐波那契数列
来源：http://tmy.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qvw.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jrh.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ayy.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uea.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hfm.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cif.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ehq.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nco.quarkkingdee.top

[N05] 最大公约数
来源：http://lxl.cashguo.top

Py:   math.gcd(a, b)
来源：http://gtb.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igq.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://src.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nip.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://amp.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zov.hfpthk.cn

Ruby: a.gcd(b)
来源：http://hdn.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lfe.sysykeji.top

[N06] 判断回文字符串
来源：http://ezq.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://yzy.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://nfl.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://wii.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://ybz.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://deg.yfazqb.com

Go:   // 双指针从两端比较
来源：http://xck.epnwcf.com

Ruby: s == s.reverse
来源：http://iwi.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gmp.yongpay.top

[N07] 两数之和（返回下标）
来源：http://imw.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yet.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aqd.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://coo.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://eqe.sxryk.cn

Java: // 手写 HashMap
来源：http://eue.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://mzy.cdnleiting.top

Ruby: // 手写 Hash
来源：http://vbq.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aoe.nanxuanxn.top

[N08] 生成全排列
来源：http://dpv.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://yzo.hnqzz.top

PHP:  // 手写递归交换
来源：http://rir.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://guj.zhengqikj.top

TS:   // 手写回溯递归
来源：http://zag.guowangkeji.top

Java: // 手写回溯递归
来源：http://poy.tianlin.xyz

Go:   // 手写回溯递归
来源：http://brk.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://xii.hnqzz.top

C#:   // 手写回溯递归
来源：http://bzi.jyoumei.cn

[N09] 栈与队列
来源：http://nca.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msu.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mlb.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lyy.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jte.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lfv.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lzs.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyt.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qsb.hnqzz.top

[N10] 链表节点定义
来源：http://tiy.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gbw.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://oat.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iwj.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afl.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://rtt.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://nze.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qjq.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jkm.xylfe.cn

[N11] 二叉树中序遍历
来源：http://efa.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pog.yuanzhike.top

PHP:  // 手写递归函数
来源：http://fzq.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esg.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mvz.fehbvm.com

Java: // 手写递归
来源：http://mwd.ehwqpu.com

Go:   // 手写递归
来源：http://tmz.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://chq.uphjek.com

C#:   // 手写递归
来源：http://cdd.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xkq.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hlv.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pqw.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tig.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kiy.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vfp.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cit.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tsq.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://njg.meibo888.top

================================================================================
来源：http://iav.fehbvm.com

O. 并发与异步
来源：http://ztp.jinqigufen.top

================================================================================
来源：http://tuc.gotoacloud.top

[O01] 启动一个线程
来源：http://lsz.ivvv.top


<!-- 参考信息 -->