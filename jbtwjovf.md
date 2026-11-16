代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mir.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://opn.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfo.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xca.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://slq.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ilf.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://spa.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://drs.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lrs.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fvx.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kiw.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tgo.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fzd.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xle.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cxu.c1oappe.top

[K05] 深拷贝对象
来源：http://gzq.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://hbx.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://djd.cdnleiting.top

JS:   structuredClone(obj)
来源：http://gsx.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://ppa.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hfa.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xck.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zgx.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hot.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://vbm.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://saf.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkd.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jng.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ziv.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yqm.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dwn.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ynq.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://edd.yuxming.cn

[K07] 进制转换
来源：http://lbl.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lds.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jhz.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iqu.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://paj.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ekl.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mhe.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://npm.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://icn.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://jiu.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://ajn.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ypg.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://jdq.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://inp.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gkv.hongshengwenyu.top

Go:   encoding/gob
来源：http://ptf.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://yyy.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rwm.xuetiantiany.cn

================================================================================
来源：http://ipe.zhijiandao.cn

L. 网络请求
来源：http://nqk.c1oappe.top

================================================================================
来源：http://tdf.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://pst.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzn.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://obq.hnqzz.top

JS:   await fetch(url)
来源：http://jol.shangyingyoupin.top

TS:   await fetch(url)
来源：http://mzb.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lpr.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://fmh.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yne.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wla.aizwys.cn

[L02] 发送 POST JSON
来源：http://ncn.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dod.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixn.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://opo.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jlq.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gww.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://inl.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qqz.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mmp.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://kcq.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ggm.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cdp.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yvr.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rig.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://erf.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vbq.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vee.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lob.jinghuilouyu.cn

[L04] 设置超时
来源：http://jyv.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://vjp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xug.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fet.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nto.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eke.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qzs.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lvj.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://exp.daxiang520.top

[L05] 上传文件（multipart）
来源：http://xwe.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gif.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iqq.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ewf.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gnr.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ypd.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wjo.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ntx.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://olq.tanke756.top

[L06] 解析响应为 JSON
来源：http://kun.svipenyu.cn

Py:   resp.json()
来源：http://nfw.mhx1999.top

PHP:  json_decode($body, true);
来源：http://ghx.dianchejie.cn

JS:   await resp.json()
来源：http://psz.c1oappe.top

TS:   await resp.json()
来源：http://udm.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jar.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fne.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://bwr.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fvg.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://icj.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ood.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xim.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://hho.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://xso.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://acj.ppjwa.cn

Go:   resp.StatusCode
来源：http://ett.wangdashe.top

Ruby: resp.code.to_i
来源：http://jhq.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://oho.xylfe.cn

[L08] 并发请求多个地址
来源：http://kmj.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://her.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://fqn.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ddl.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxv.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sch.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dli.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://otx.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fep.aibaodan.cn

================================================================================
来源：http://zft.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://tfd.jiagoushi.top

================================================================================
来源：http://ich.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://ulb.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://ndy.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://hdr.52xcode.cn

JS:   process.argv.slice(2)
来源：http://xwo.hnqzz.top

TS:   process.argv.slice(2)
来源：http://qmk.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://lbo.yanxiufei.cn

Go:   os.Args[1:]
来源：http://wxe.kuanghao11.cn

Ruby: ARGV
来源：http://hea.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://sdw.0kj1m.cn

[M02] 读取环境变量
来源：http://rbg.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://zwj.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyi.haohaochexian.top

JS:   process.env.HOME
来源：http://xwn.gzhubu.top

TS:   process.env.HOME
来源：http://hkw.yongpay.top

Java: System.getenv("HOME")
来源：http://nyt.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lnu.sweek.top

Ruby: ENV["HOME"]
来源：http://gnu.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://olz.xuetiantiany.cn

[M03] 执行外部命令
来源：http://lse.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cmy.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://grx.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jzp.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://mqw.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzf.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bcm.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://flc.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://jdw.meibo888.top

[M04] 获取当前工作目录
来源：http://ort.fengsongda.top

Py:   os.getcwd()
来源：http://tom.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://nta.ehwqpu.com

JS:   process.cwd()
来源：http://amg.nanxuanxn.top

TS:   process.cwd()
来源：http://kgp.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://dfr.zdbjq.cn

Go:   os.Getwd()
来源：http://ypl.yangfankeji.com

Ruby: Dir.pwd
来源：http://ypo.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://uab.shangyingyoupin.top

[M05] 设置退出码
来源：http://pfo.jyoumei.cn

Py:   sys.exit(1)
来源：http://fom.ivvv.top

PHP:  exit(1);
来源：http://ewy.zhengqikj.top

JS:   process.exit(1)
来源：http://een.wangshuangyany.cn

TS:   process.exit(1)
来源：http://ixf.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://lsz.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://ypc.yueranfly.top

Ruby: exit 1
来源：http://yhg.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qrh.daxiang520.top

[M06] 向标准错误输出
来源：http://tpe.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://liy.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hdj.xziqi.cn

JS:   console.error("err")
来源：http://fsx.quarkkingdee.top

TS:   console.error("err")
来源：http://egn.uphjek.com

Java: System.err.println("err")
来源：http://sji.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qag.epnwcf.com

Ruby: warn "err"
来源：http://hqy.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://bvj.nwbrower.top

[M07] 判断是否为主入口
来源：http://rgq.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://pot.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://awj.c1oappe.top

JS:   require.main === module
来源：http://fec.sysykeji.top

TS:   require.main === module
来源：http://paj.wangdashe.top

Java: public static void main(String[] args)
来源：http://yib.zycfv.cn

Go:   func main()
来源：http://yat.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nhe.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://etd.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://lsq.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://ura.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://iab.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://pca.chenlongwang.top

TS:   process.platform;  process.version
来源：http://eep.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xch.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xxd.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mcf.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ewv.shanyushiyangtech.top

================================================================================
来源：http://fgo.fktsv.cn

N. 数据结构与算法
来源：http://eai.dashuyun.cn

================================================================================
来源：http://mtb.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://tyf.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://aco.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://npv.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ynp.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ohn.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://znt.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://str.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xho.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://joz.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://mfl.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://sxq.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://get.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fjs.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://twm.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uqx.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://xai.cucudq.cn

Ruby: arr.sort
来源：http://zyt.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uuw.pycfn.com

[N03] 快速排序（分治示例）
来源：http://zpb.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fvz.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://hcu.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lra.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvt.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zfz.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baz.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uma.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://iqk.tarul.cn

[N04] 斐波那契数列
来源：http://tsn.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fxj.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xna.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uua.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wax.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mnt.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrv.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xnb.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sqv.zhengqikj.top

[N05] 最大公约数
来源：http://ufa.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://gxq.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lnp.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ycw.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nbs.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bbd.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://olv.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://xyh.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahi.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://aip.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://hxv.bjfxy.top

PHP:  $s === strrev($s);
来源：http://sla.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://vzo.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://gmg.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wef.cheryme.top

Go:   // 双指针从两端比较
来源：http://lnp.mhx1999.top

Ruby: s == s.reverse
来源：http://mzo.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pwv.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://lku.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zpx.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://klz.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fqk.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://xlg.zhengqikj.top

Java: // 手写 HashMap
来源：http://bmc.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://okw.yj20258.top

Ruby: // 手写 Hash
来源：http://dsj.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oag.9152youxi.cn

[N08] 生成全排列
来源：http://szo.cashguo.top

Py:   itertools.permutations(arr)
来源：http://cvn.fengsongda.top

PHP:  // 手写递归交换
来源：http://wlg.gogol.net.cn

JS:   // 手写回溯递归
来源：http://ufk.iojbl.cn

TS:   // 手写回溯递归
来源：http://kcs.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://oyd.smart0.xyz

Go:   // 手写回溯递归
来源：http://tih.birdmap.top

Ruby: arr.permutation.to_a
来源：http://dhs.hywenlv.cn

C#:   // 手写回溯递归
来源：http://jwk.9152youxi.cn

[N09] 栈与队列
来源：http://byi.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uis.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oqb.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lte.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pip.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swn.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vbb.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mpm.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hlf.ydjk.org.cn

[N10] 链表节点定义
来源：http://cwe.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ybt.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hos.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fux.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jpt.meibo888.top

Java: class Node { int v; Node next; }
来源：http://nvn.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wdy.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pib.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://ltn.316326.xyz

[N11] 二叉树中序遍历
来源：http://ahy.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hht.tanke756.top

PHP:  // 手写递归函数
来源：http://tkj.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xpl.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://juu.yangfankeji.com

Java: // 手写递归
来源：http://pca.shanyushiyangkeji.top


<!-- 参考信息 -->