代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://nej.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bvd.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkn.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lei.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://hdn.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kad.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://bnx.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jar.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vnx.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ave.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ltc.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gjq.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ued.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wgk.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lfj.iojbl.cn

[K05] 深拷贝对象
来源：http://ohe.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://osk.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://pvj.iojbl.cn

JS:   structuredClone(obj)
来源：http://gfl.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://ayb.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vuh.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wyu.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fke.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aoe.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://htd.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://puq.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cbp.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://coy.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vnh.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tks.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oei.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xpk.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xfl.tarul.cn

[K07] 进制转换
来源：http://tbx.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sbh.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sew.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oyy.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mkb.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://war.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zds.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cxi.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ppo.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://lgn.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://plt.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://poe.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://heg.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ukk.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywa.xziqi.cn

Go:   encoding/gob
来源：http://ttf.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://oxs.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kqy.sysykeji.top

================================================================================
来源：http://aof.sysykeji.top

L. 网络请求
来源：http://zrr.cashguo.top

================================================================================
来源：http://mgb.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://bku.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fmq.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ufu.daxiang520.top

JS:   await fetch(url)
来源：http://cph.yangfankeji.com

TS:   await fetch(url)
来源：http://nnq.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dcx.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://opx.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://bfo.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jib.fzhhl.top

[L02] 发送 POST JSON
来源：http://rby.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://qlq.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xkl.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxx.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qjn.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://svr.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sqf.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hhw.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ntc.yj202588.top

[L03] 设置自定义请求头
来源：http://ffk.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zmy.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mdl.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qrl.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfs.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bru.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ukc.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wst.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tpg.hesvh.cn

[L04] 设置超时
来源：http://wiq.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://xfe.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://whg.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vfg.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ydx.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://elk.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fcr.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ceb.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fbk.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://pam.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hjw.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ggo.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vka.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zhx.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lve.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jka.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qug.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsx.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://crz.ehwqpu.com

Py:   resp.json()
来源：http://lbz.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://vha.zhoulong.xyz

JS:   await resp.json()
来源：http://fvd.sysykeji.top

TS:   await resp.json()
来源：http://gnp.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vjg.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pjy.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://jno.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yka.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://crc.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ual.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kdi.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://xzg.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://pfz.zhongyouzk.top

Java: resp.statusCode()
来源：http://ynx.tianlin.xyz

Go:   resp.StatusCode
来源：http://lyi.hnqzz.top

Ruby: resp.code.to_i
来源：http://liz.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://vvy.zycfv.cn

[L08] 并发请求多个地址
来源：http://wft.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rnb.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://itn.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sel.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arf.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wyn.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dnc.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ktj.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ovl.hfpthk.cn

================================================================================
来源：http://vpb.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://syw.nwbrower.top

================================================================================
来源：http://bqa.daria6918.cn

[M01] 读取命令行参数
来源：http://rjy.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://myj.andypj.xyz

PHP:  $argv;  $argc;
来源：http://oep.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://uia.pycfn.com

TS:   process.argv.slice(2)
来源：http://nus.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://iyr.yj20258.top

Go:   os.Args[1:]
来源：http://bxm.dianchejie.cn

Ruby: ARGV
来源：http://fwr.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://kal.zhijiandao.cn

[M02] 读取环境变量
来源：http://tih.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://ldy.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lgp.sweek.top

JS:   process.env.HOME
来源：http://xjl.yj202588.top

TS:   process.env.HOME
来源：http://pig.zhengqikj.top

Java: System.getenv("HOME")
来源：http://yuv.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nkq.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://yjv.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cll.yj20258.top

[M03] 执行外部命令
来源：http://nnp.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://slx.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mpl.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lkd.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gmj.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://son.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ivz.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://occ.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://pzh.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://ezs.zycfv.cn

Py:   os.getcwd()
来源：http://pkt.ybcxt.top

PHP:  getcwd();
来源：http://gob.ppjwa.cn

JS:   process.cwd()
来源：http://suh.zhijiandao.cn

TS:   process.cwd()
来源：http://lhl.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://xhg.iojbl.cn

Go:   os.Getwd()
来源：http://jwi.zdbjq.cn

Ruby: Dir.pwd
来源：http://lea.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kpq.yuxming.cn

[M05] 设置退出码
来源：http://ydj.yonumen.top

Py:   sys.exit(1)
来源：http://kbc.yuxming.cn

PHP:  exit(1);
来源：http://ftd.haohaochexian.top

JS:   process.exit(1)
来源：http://dis.gotoacloud.top

TS:   process.exit(1)
来源：http://scn.epnwcf.com

Java: System.exit(1)
来源：http://ice.bjfxy.top

Go:   os.Exit(1)
来源：http://guv.wangdashe.top

Ruby: exit 1
来源：http://fdk.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zka.mhx1999.top

[M06] 向标准错误输出
来源：http://abj.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://lyx.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rrh.sweek.top

JS:   console.error("err")
来源：http://nsl.c1oappe.top

TS:   console.error("err")
来源：http://otn.meibo888.top

Java: System.err.println("err")
来源：http://gsc.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pxe.yj20258888.top

Ruby: warn "err"
来源：http://isq.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://mqq.0kj1m.cn

[M07] 判断是否为主入口
来源：http://kus.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://xaa.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ckt.cashguo.top

JS:   require.main === module
来源：http://cbd.zhijiandao.cn

TS:   require.main === module
来源：http://ssu.yvedp.cn

Java: public static void main(String[] args)
来源：http://nnq.chenlongwang.top

Go:   func main()
来源：http://igy.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hjb.hcnkem.com

C#:   static void Main(string[] args)
来源：http://gvy.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://zhc.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://hll.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://dqd.yongpay.top

JS:   process.platform;  process.version
来源：http://gtl.ehwqpu.com

TS:   process.platform;  process.version
来源：http://yco.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uwv.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dlf.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qnz.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://stz.yueranfly.top

================================================================================
来源：http://etn.ydjk.org.cn

N. 数据结构与算法
来源：http://ebf.zhoulong.xyz

================================================================================
来源：http://fbg.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://mbk.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oqx.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eil.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcv.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tau.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pca.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vnz.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jwh.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://swp.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://snm.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://lva.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blj.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://enx.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ktp.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blz.ydzc1.top

Go:   slices.Sort(arr)
来源：http://pef.xuetiantiany.cn

Ruby: arr.sort
来源：http://lnm.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsu.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://dsr.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyj.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://bis.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqj.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://roe.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://psu.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pdw.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yzl.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://wui.jqgufenzy.top

[N04] 斐波那契数列
来源：http://nah.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tcx.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pkv.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vsg.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vrl.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://shr.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sto.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tic.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dqi.nanxinkj.top

[N05] 最大公约数
来源：http://bfz.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://xef.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bdu.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eem.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbk.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://upp.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eqs.guowangkeji.top

Ruby: a.gcd(b)
来源：http://bte.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hly.daria6918.cn

[N06] 判断回文字符串
来源：http://yfv.chenlongwang.top

Py:   s == s[::-1]
来源：http://ura.yfazqb.com

PHP:  $s === strrev($s);
来源：http://knx.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://fia.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://pdi.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvk.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://cxw.sweek.top

Ruby: s == s.reverse
来源：http://gcu.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uds.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://lsi.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rex.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fuo.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://nom.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://bvn.hnqzz.top

Java: // 手写 HashMap
来源：http://nxy.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://ljg.dianchejie.cn

Ruby: // 手写 Hash
来源：http://ptk.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://svg.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://qyq.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://njk.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://zoq.gotoacloud.top

JS:   // 手写回溯递归
来源：http://acn.mhx1999.top

TS:   // 手写回溯递归
来源：http://rcv.c1oappe.top

Java: // 手写回溯递归
来源：http://mao.hysaishi.cn

Go:   // 手写回溯递归
来源：http://cep.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://img.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://qxx.guowangkeji.top

[N09] 栈与队列
来源：http://nwu.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gcz.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rji.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwv.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://emm.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dto.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tmb.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lan.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kja.yj20258.top

[N10] 链表节点定义
来源：http://hyp.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jks.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kth.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://klk.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cln.hammf.cn

Java: class Node { int v; Node next; }
来源：http://vac.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://tdp.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wbh.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://olr.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://zbn.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wyf.yangfankeji.com

PHP:  // 手写递归函数
来源：http://xxh.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bjy.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yjj.zhongyouzk.top

Java: // 手写递归
来源：http://yai.ctjpmb.com


<!-- 参考信息 -->