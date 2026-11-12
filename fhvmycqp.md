代发 wailian999

TS:   JSON.parse(s)
来源：http://xgw.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kyk.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://kvi.bjfxy.top

Ruby: JSON.parse(s)
来源：http://kij.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://akv.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://wzi.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jcg.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lsn.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ocv.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ifw.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sqx.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yuf.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://ufb.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://isn.yueranfly.top

[K04] 读取 JSON 文件
来源：http://qmn.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tak.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwa.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zqf.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://duz.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hdt.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bht.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sra.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://txd.ppjwa.cn

[K05] 深拷贝对象
来源：http://loa.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://jcf.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://syn.iojbl.cn

JS:   structuredClone(obj)
来源：http://sxw.hesvh.cn

TS:   structuredClone(obj)
来源：http://hub.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lvb.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zpz.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdr.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oid.aizwys.cn

[K06] 解析 URL 查询串
来源：http://fye.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nhj.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pga.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnf.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rov.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wdo.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://flf.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fmp.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zgl.yuxming.cn

[K07] 进制转换
来源：http://jvx.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxm.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oou.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sgn.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bqa.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mad.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vlz.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://voe.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lgb.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://qgp.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://eob.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://auh.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://pzu.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://zgo.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xjq.daxiang520.top

Go:   encoding/gob
来源：http://adk.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://ugc.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bkd.jiagoushi.top

================================================================================
来源：http://ceq.zycfv.cn

L. 网络请求
来源：http://udy.hysaishi.cn

================================================================================
来源：http://uic.hammf.cn

[L01] 发送 GET 请求
来源：http://gjz.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jws.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dmp.xuanzx.com

JS:   await fetch(url)
来源：http://euf.uphjek.com

TS:   await fetch(url)
来源：http://xcb.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://exc.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://itk.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ynf.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jan.316326.xyz

[L02] 发送 POST JSON
来源：http://kui.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xoj.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wor.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://egm.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyz.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rhs.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hsn.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bty.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dqv.shzxlz.cn

[L03] 设置自定义请求头
来源：http://jfi.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jle.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://enx.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kvj.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpg.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://brt.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://imo.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yyt.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dva.gzhubu.top

[L04] 设置超时
来源：http://fqd.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://bbq.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uqr.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhm.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ung.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bwv.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bjj.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gcb.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ifc.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://jge.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ohv.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hic.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qlv.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ato.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://urx.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://clm.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ozt.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckm.yueranfly.top

[L06] 解析响应为 JSON
来源：http://jng.yj20258888.top

Py:   resp.json()
来源：http://uaf.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://mdw.redwolf501.top

JS:   await resp.json()
来源：http://ahy.aibaodan.cn

TS:   await resp.json()
来源：http://vtq.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://itj.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dgf.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://ogg.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tsl.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://ixg.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bju.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ojm.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://lld.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://fbz.yvedp.cn

Java: resp.statusCode()
来源：http://hes.sweek.top

Go:   resp.StatusCode
来源：http://xfx.hesvh.cn

Ruby: resp.code.to_i
来源：http://asg.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://doz.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://vdu.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ovr.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://rsq.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gfp.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozn.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cux.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kqh.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hha.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ebg.hywenlv.cn

================================================================================
来源：http://kdp.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://nay.zhixingplan.top

================================================================================
来源：http://nsl.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://egj.hesvh.cn

Py:   sys.argv[1:]
来源：http://veo.yfazqb.com

PHP:  $argv;  $argc;
来源：http://joo.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://cuh.shuidangran.top

TS:   process.argv.slice(2)
来源：http://sgp.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://lca.hammf.cn

Go:   os.Args[1:]
来源：http://emm.ctjpmb.com

Ruby: ARGV
来源：http://pfl.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://jum.xylfe.cn

[M02] 读取环境变量
来源：http://jlp.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://ask.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mcb.xuanzx.com

JS:   process.env.HOME
来源：http://jsb.yueranfly.top

TS:   process.env.HOME
来源：http://ovi.vehdjk.com

Java: System.getenv("HOME")
来源：http://pbr.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhz.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://tpg.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qfd.yanxiufei.cn

[M03] 执行外部命令
来源：http://drb.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tgo.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lao.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tfv.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jaf.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ypv.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zzb.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://rff.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://ybh.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://njg.hnxiangtu.top

Py:   os.getcwd()
来源：http://vet.yfazqb.com

PHP:  getcwd();
来源：http://cnm.pycfn.com

JS:   process.cwd()
来源：http://yfl.fanxiaobao.xyz

TS:   process.cwd()
来源：http://mji.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://jnd.mhx1999.top

Go:   os.Getwd()
来源：http://hxq.vqdsnc.cn

Ruby: Dir.pwd
来源：http://izw.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://bmk.316326.xyz

[M05] 设置退出码
来源：http://trt.hysaishi.cn

Py:   sys.exit(1)
来源：http://yzz.mhx1999.top

PHP:  exit(1);
来源：http://ibc.fehbvm.com

JS:   process.exit(1)
来源：http://qmk.jiagoushi.top

TS:   process.exit(1)
来源：http://nzx.sufxvd.cn

Java: System.exit(1)
来源：http://wmx.hammf.cn

Go:   os.Exit(1)
来源：http://dwt.chenzaomai.com

Ruby: exit 1
来源：http://tec.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://stk.daxiang520.top

[M06] 向标准错误输出
来源：http://afq.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://gym.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://agn.0kj1m.cn

JS:   console.error("err")
来源：http://yqq.birdmap.top

TS:   console.error("err")
来源：http://drx.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://ota.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ebk.hammf.cn

Ruby: warn "err"
来源：http://pjv.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ris.birdmap.top

[M07] 判断是否为主入口
来源：http://uqw.uphjek.com

Py:   if __name__ == "__main__":
来源：http://rqo.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://evp.yanxiufei.cn

JS:   require.main === module
来源：http://kdd.fehbvm.com

TS:   require.main === module
来源：http://icz.guannengcc.top

Java: public static void main(String[] args)
来源：http://sci.9152youxi.cn

Go:   func main()
来源：http://yyn.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://toa.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://vat.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://iuf.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://ydt.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://qvl.hcnkem.com

JS:   process.platform;  process.version
来源：http://aay.snrcjt.cn

TS:   process.platform;  process.version
来源：http://iin.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mor.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://njo.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gvg.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gda.jqgfzy.top

================================================================================
来源：http://zmz.jianghu66.top

N. 数据结构与算法
来源：http://xpz.gogol.net.cn

================================================================================
来源：http://thm.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://rvo.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iht.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cza.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmb.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xpa.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hbk.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://xti.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ypd.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://tme.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://wzm.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://boi.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqe.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mja.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jkg.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://roq.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://nip.sweek.top

Ruby: arr.sort
来源：http://wzi.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rpx.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://rpc.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ulb.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://wng.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fka.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zcv.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ejw.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vpr.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whb.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://rjx.nwbrower.top

[N04] 斐波那契数列
来源：http://jex.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nmw.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uww.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylw.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eep.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nhz.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fia.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kom.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cvb.zhijiandao.cn

[N05] 最大公约数
来源：http://tih.jianghu66.top

Py:   math.gcd(a, b)
来源：http://xcn.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://csn.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sts.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dua.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cph.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://upo.jianghu66.top

Ruby: a.gcd(b)
来源：http://erq.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pje.fehbvm.com

[N06] 判断回文字符串
来源：http://lfv.shuidangran.top

Py:   s == s[::-1]
来源：http://nxx.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://cnf.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://six.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://yoy.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iug.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://nzs.zdqjudy.top

Ruby: s == s.reverse
来源：http://bbs.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yly.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://ntg.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nza.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hkh.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://prk.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://ndk.yj20258.top

Java: // 手写 HashMap
来源：http://hpx.bbcook.cn

Go:   // 手写 map[int]int
来源：http://tko.cqqwz.cn

Ruby: // 手写 Hash
来源：http://hwl.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vpv.xuetiantiany.cn

[N08] 生成全排列
来源：http://jir.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://srz.mhx1999.top

PHP:  // 手写递归交换
来源：http://mdy.ctjpmb.com

JS:   // 手写回溯递归
来源：http://htf.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://pcm.sweek.top

Java: // 手写回溯递归
来源：http://qtf.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://lgo.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://laj.xinyue.icu

C#:   // 手写回溯递归
来源：http://xjs.uphjek.com

[N09] 栈与队列
来源：http://phw.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qrv.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xvj.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ima.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uxs.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hgk.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fnj.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kyw.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qdp.epnwcf.com

[N10] 链表节点定义
来源：http://ssr.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vuj.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://arb.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tbd.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oow.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://dlx.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kjc.mhx1999.top


<!-- 参考信息 -->