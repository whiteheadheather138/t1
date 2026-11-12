代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gvk.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wdi.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lyo.shuidangran.top

[K05] 深拷贝对象
来源：http://scp.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://rms.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://bxl.hesvh.cn

JS:   structuredClone(obj)
来源：http://rxi.dianchejie.cn

TS:   structuredClone(obj)
来源：http://edc.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yto.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xxf.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jiq.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gcg.yj20258888.top

[K06] 解析 URL 查询串
来源：http://rfr.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nco.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ybi.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfr.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rxp.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://llo.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oyq.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ovu.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mtv.yfazqb.com

[K07] 进制转换
来源：http://ntm.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nau.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kxv.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nxn.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gvs.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hxk.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://txm.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qzh.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://czs.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://gcw.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://ihg.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lhp.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://aeg.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://rbk.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://row.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://agt.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://tuh.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wfk.dianchejie.cn

================================================================================
来源：http://fdk.jinyuanbaomall.cn

L. 网络请求
来源：http://sbp.ybcxt.top

================================================================================
来源：http://xwo.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://sca.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqh.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lea.ppjwa.cn

JS:   await fetch(url)
来源：http://bqn.9152youxi.cn

TS:   await fetch(url)
来源：http://gml.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uda.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://www.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xbl.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xjh.hfpthk.cn

[L02] 发送 POST JSON
来源：http://rxg.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cao.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hqo.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://moh.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqn.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://loo.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cgc.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://krc.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ozh.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://kyx.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wdn.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hwd.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fgt.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijr.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://etq.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uls.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pnk.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lda.zhengqikj.top

[L04] 设置超时
来源：http://vlp.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://qhi.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://glh.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwc.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hek.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yei.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iye.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lhz.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pna.xuanzx.com

[L05] 上传文件（multipart）
来源：http://jlj.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zsu.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qdg.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kwp.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iuk.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xho.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gvm.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://exy.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://doa.52xcode.cn

[L06] 解析响应为 JSON
来源：http://jlr.jlsjyb.cn

Py:   resp.json()
来源：http://nii.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://wbq.hesvh.cn

JS:   await resp.json()
来源：http://ruw.fengsongda.top

TS:   await resp.json()
来源：http://qed.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://all.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nao.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ewp.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wuw.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://kws.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nbg.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qll.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://mcd.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://kfo.chenjidiqi.icu

Java: resp.statusCode()
来源：http://sni.tarul.cn

Go:   resp.StatusCode
来源：http://key.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://hzw.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://fln.dashuyun.cn

[L08] 并发请求多个地址
来源：http://pji.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vex.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://esp.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://njt.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cet.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zxw.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hnr.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oyw.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nkf.guannengcc.top

================================================================================
来源：http://lkn.sweek.top

M. 命令行 / 进程 / 环境
来源：http://dlg.jinqigfzy.top

================================================================================
来源：http://gli.nanxuanxn.top

[M01] 读取命令行参数
来源：http://rhm.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://hlt.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://sbo.tian-w.cn

JS:   process.argv.slice(2)
来源：http://nxz.fzhhl.top

TS:   process.argv.slice(2)
来源：http://gmm.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://ixf.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://jdb.cheryme.top

Ruby: ARGV
来源：http://yqm.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://ttl.bjfxy.top

[M02] 读取环境变量
来源：http://xpb.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://tvn.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ksq.ehwqpu.com

JS:   process.env.HOME
来源：http://adc.zdqjudy.top

TS:   process.env.HOME
来源：http://hey.zdbjq.cn

Java: System.getenv("HOME")
来源：http://ywh.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dmp.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://kvv.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uww.jqgfzy.top

[M03] 执行外部命令
来源：http://xqb.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rbh.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qnl.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ank.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fmf.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nyy.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rwp.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://tpp.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://klz.hnqzz.top

[M04] 获取当前工作目录
来源：http://rmf.zhengqikj.top

Py:   os.getcwd()
来源：http://esp.yfazqb.com

PHP:  getcwd();
来源：http://dgo.fehbvm.com

JS:   process.cwd()
来源：http://jqq.jyoumei.cn

TS:   process.cwd()
来源：http://eqx.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://uud.yj20258.top

Go:   os.Getwd()
来源：http://hkl.vehdjk.com

Ruby: Dir.pwd
来源：http://tim.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://byl.zhoulong.xyz

[M05] 设置退出码
来源：http://cru.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://peo.0kj1m.cn

PHP:  exit(1);
来源：http://nxa.meibo888.top

JS:   process.exit(1)
来源：http://qhv.redwolf501.top

TS:   process.exit(1)
来源：http://bey.jyoumei.cn

Java: System.exit(1)
来源：http://dvh.daria6918.cn

Go:   os.Exit(1)
来源：http://rvv.yj20258888.top

Ruby: exit 1
来源：http://xmi.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wqy.iojbl.cn

[M06] 向标准错误输出
来源：http://vfy.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://wyw.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qmt.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://lrr.yvedp.cn

TS:   console.error("err")
来源：http://syp.chenlongwang.top

Java: System.err.println("err")
来源：http://nze.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mdx.xinyue.icu

Ruby: warn "err"
来源：http://jdg.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://xhc.ppjwa.cn

[M07] 判断是否为主入口
来源：http://llx.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://zhg.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://poz.jyoumei.cn

JS:   require.main === module
来源：http://xnj.vehdjk.com

TS:   require.main === module
来源：http://fkf.ppjwa.cn

Java: public static void main(String[] args)
来源：http://chq.jianghu66.top

Go:   func main()
来源：http://oin.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bud.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://leh.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://knw.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://pqb.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://ycv.bbcook.cn

JS:   process.platform;  process.version
来源：http://ruo.9152youxi.cn

TS:   process.platform;  process.version
来源：http://bxw.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nec.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gem.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxs.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tjq.hywenlv.cn

================================================================================
来源：http://moj.jqgufenzy.top

N. 数据结构与算法
来源：http://gwb.gotoacloud.top

================================================================================
来源：http://rox.meibo888.top

[N01] 二分查找（有序数组）
来源：http://png.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ihy.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yxe.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxq.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czi.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xez.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://qkx.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xke.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iis.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://snd.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://hvj.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogz.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://put.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pnr.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iro.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://azg.yuanzhike.top

Ruby: arr.sort
来源：http://ssw.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://amq.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://ses.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vtk.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://cks.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://evi.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wpt.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tch.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wxm.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yzn.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://tci.chenzaomai.com

[N04] 斐波那契数列
来源：http://ffe.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qmx.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zlx.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opn.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buc.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ary.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tds.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jng.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iki.fengsongda.top

[N05] 最大公约数
来源：http://aqf.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://wwp.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iux.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gmk.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://woi.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gni.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://usy.aibaodan.cn

Ruby: a.gcd(b)
来源：http://rqo.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hrv.jinqigfzy.top

[N06] 判断回文字符串
来源：http://szi.hywenlv.cn

Py:   s == s[::-1]
来源：http://lyl.tarul.cn

PHP:  $s === strrev($s);
来源：http://bcw.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://sam.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://pob.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ydi.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://ypk.jiagoushi.top

Ruby: s == s.reverse
来源：http://hkr.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://sny.316326.xyz

[N07] 两数之和（返回下标）
来源：http://fsb.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://djo.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wwy.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xjd.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://uqc.hysaishi.cn

Java: // 手写 HashMap
来源：http://lpc.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://zqw.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://ywk.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://rmu.yvedp.cn

[N08] 生成全排列
来源：http://wks.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://hjt.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://wab.yueranfly.top

JS:   // 手写回溯递归
来源：http://vvo.fengsongda.top

TS:   // 手写回溯递归
来源：http://woq.guowangkeji.top

Java: // 手写回溯递归
来源：http://ooq.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://vtc.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://sus.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://lfl.zdqjudy.top

[N09] 栈与队列
来源：http://gki.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ztz.wangshuangyany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rng.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://omx.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qxa.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fmi.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cqt.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qex.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cjv.0kj1m.cn

[N10] 链表节点定义
来源：http://tln.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qxg.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ylp.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nvs.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://huc.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://kqw.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zgk.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ykz.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://npx.andypj.xyz

[N11] 二叉树中序遍历
来源：http://qnf.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gqv.ppjwa.cn

PHP:  // 手写递归函数
来源：http://vfr.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxk.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tet.hongshengwenyu.top

Java: // 手写递归
来源：http://dpu.chenzaomai.com

Go:   // 手写递归
来源：http://gri.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nqx.redwolf501.top

C#:   // 手写递归
来源：http://tpq.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yuy.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nxj.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bya.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mko.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruf.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ger.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vwc.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ibj.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ien.hesvh.cn


<!-- 参考信息 -->