代发 wailian999

TS:   JSON.parse(s)
来源：http://gmu.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iie.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://zen.bjfxy.top

Ruby: JSON.parse(s)
来源：http://ovg.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mml.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qdy.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jwb.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lho.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bry.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kgh.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vig.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wtm.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://rti.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xps.fehbvm.com

[K04] 读取 JSON 文件
来源：http://ykn.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nbo.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ovt.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kiz.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnk.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ckn.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxp.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pxd.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zsf.bjfxy.top

[K05] 深拷贝对象
来源：http://obk.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://ndm.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://gmm.cdnleiting.top

JS:   structuredClone(obj)
来源：http://cob.zhengqikj.top

TS:   structuredClone(obj)
来源：http://cjv.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xrr.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qyq.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zic.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://duw.daria6918.cn

[K06] 解析 URL 查询串
来源：http://sxp.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjv.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zmy.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hjs.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kfv.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zby.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://njy.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cra.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rfb.jlsjyb.cn

[K07] 进制转换
来源：http://itm.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://owh.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ijg.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jgu.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://amq.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vgt.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kxz.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mbm.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ffq.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://zxs.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://oaf.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ngq.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://zax.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://moi.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dws.gaohongyu789.top

Go:   encoding/gob
来源：http://vnb.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://nkj.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xok.haohaochexian.top

================================================================================
来源：http://dhu.yj20258.top

L. 网络请求
来源：http://jxe.yangfankeji.com

================================================================================
来源：http://leq.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://xdl.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://prw.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cfi.pengpengdd.cyou

JS:   await fetch(url)
来源：http://rck.dashuyun.cn

TS:   await fetch(url)
来源：http://pcm.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://crl.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://kkm.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uja.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jrl.cucudq.cn

[L02] 发送 POST JSON
来源：http://iae.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://yzb.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fpg.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhl.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkj.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://twn.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hcs.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fmh.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kbp.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://mnm.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pba.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://spe.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxu.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jff.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://poo.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kit.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eay.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zpu.yuanzhike.top

[L04] 设置超时
来源：http://bdn.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://mrz.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tfz.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vys.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bfi.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xpj.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ves.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://leq.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bbf.havefunace.top

[L05] 上传文件（multipart）
来源：http://mgu.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hge.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iol.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wga.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bve.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sux.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lov.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hov.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wqa.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://dix.chenjidiqi.icu

Py:   resp.json()
来源：http://esi.redwolf501.top

PHP:  json_decode($body, true);
来源：http://dos.jlsjyb.cn

JS:   await resp.json()
来源：http://hue.sysykeji.top

TS:   await resp.json()
来源：http://jbo.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://geh.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jgx.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://mkk.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://geq.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://fwq.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tms.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vcf.tarul.cn

JS:   resp.ok;  resp.status
来源：http://ayr.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://nfh.zhiwuduotai.top

Java: resp.statusCode()
来源：http://fas.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://uod.cdnleiting.top

Ruby: resp.code.to_i
来源：http://vjj.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://tdu.jiagoushi.top

[L08] 并发请求多个地址
来源：http://pnd.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eat.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://uoa.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://csy.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dsd.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://luy.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hvu.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ceg.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://esy.shuidangran.top

================================================================================
来源：http://bff.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://lyt.jqgufenzy.top

================================================================================
来源：http://vht.zhoulong.xyz

[M01] 读取命令行参数
来源：http://pss.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://aes.tian-w.cn

PHP:  $argv;  $argc;
来源：http://irc.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://uap.xuanzx.com

TS:   process.argv.slice(2)
来源：http://vsf.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://wsw.sweek.top

Go:   os.Args[1:]
来源：http://ijf.ivvv.top

Ruby: ARGV
来源：http://key.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://tdu.gotoacloud.top

[M02] 读取环境变量
来源：http://svo.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://ieu.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xae.guannengcc.top

JS:   process.env.HOME
来源：http://axd.meibo888.top

TS:   process.env.HOME
来源：http://iil.sweek.top

Java: System.getenv("HOME")
来源：http://whk.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zhr.yonumen.top

Ruby: ENV["HOME"]
来源：http://rxe.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ukz.cashguo.top

[M03] 执行外部命令
来源：http://bez.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://csk.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://arw.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qkv.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ggr.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://etf.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jgf.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cfq.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://pos.zhixingplan.top

[M04] 获取当前工作目录
来源：http://wxy.fengsongda.top

Py:   os.getcwd()
来源：http://ldx.yangfankeji.com

PHP:  getcwd();
来源：http://ohk.jinghuilouyu.cn

JS:   process.cwd()
来源：http://ato.hnqzz.top

TS:   process.cwd()
来源：http://sdd.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://nbx.shangyingyoupin.top

Go:   os.Getwd()
来源：http://eks.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://yxw.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nkz.aizwys.cn

[M05] 设置退出码
来源：http://qtv.xinyue.icu

Py:   sys.exit(1)
来源：http://mbj.wangdashe.top

PHP:  exit(1);
来源：http://rqk.fzhhl.top

JS:   process.exit(1)
来源：http://ywd.haohaochexian.top

TS:   process.exit(1)
来源：http://qjw.jlsjyb.cn

Java: System.exit(1)
来源：http://znb.c1oappe.top

Go:   os.Exit(1)
来源：http://zvq.hywenlv.cn

Ruby: exit 1
来源：http://spn.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xjj.jianghu66.top

[M06] 向标准错误输出
来源：http://eqr.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://uiq.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bbg.yuxming.cn

JS:   console.error("err")
来源：http://lvl.shanyushiyangtech.top

TS:   console.error("err")
来源：http://fuc.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://rem.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lbc.jianghu66.top

Ruby: warn "err"
来源：http://miq.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://bso.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://cfg.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://vzw.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ozr.gaohongyu789.top

JS:   require.main === module
来源：http://aps.yvedp.cn

TS:   require.main === module
来源：http://mcy.aizwys.cn

Java: public static void main(String[] args)
来源：http://bvv.havefunace.top

Go:   func main()
来源：http://bhk.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vmt.fehbvm.com

C#:   static void Main(string[] args)
来源：http://hyq.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://gnv.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://xlq.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://dnm.vehdjk.com

JS:   process.platform;  process.version
来源：http://jeu.nwbrower.top

TS:   process.platform;  process.version
来源：http://van.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fps.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lcb.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dfg.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://haj.jyoumei.cn

================================================================================
来源：http://vem.hysaishi.cn

N. 数据结构与算法
来源：http://lni.sufxvd.cn

================================================================================
来源：http://ozg.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://lng.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://flh.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bdc.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxr.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mtb.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://yfn.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xrm.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wip.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://avs.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://hvi.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vor.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nnx.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://edg.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rgu.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zhy.fengsongda.top

Go:   slices.Sort(arr)
来源：http://zih.fehbvm.com

Ruby: arr.sort
来源：http://naq.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gvc.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://hez.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wqa.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://rcy.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bep.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eor.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rkm.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xhu.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ovv.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ckm.quarkkingdee.top

[N04] 斐波那契数列
来源：http://vyb.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pbe.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wmw.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dvl.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ufq.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://him.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ojb.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvn.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xze.guannengcc.top

[N05] 最大公约数
来源：http://nxq.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://oew.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://drn.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nnm.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vhm.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cng.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kpr.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://pro.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eij.hcnkem.com

[N06] 判断回文字符串
来源：http://ldk.52xcode.cn

Py:   s == s[::-1]
来源：http://vvv.bbcook.cn

PHP:  $s === strrev($s);
来源：http://hqv.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://qwi.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://wfq.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bea.iojbl.cn

Go:   // 双指针从两端比较
来源：http://erl.cheryme.top

Ruby: s == s.reverse
来源：http://ttw.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ejs.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://lmh.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bsy.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pwb.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xef.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://fnp.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://naj.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://gtg.jianghu66.top

Ruby: // 手写 Hash
来源：http://wck.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://kma.sxryk.cn

[N08] 生成全排列
来源：http://soh.uphjek.com

Py:   itertools.permutations(arr)
来源：http://ylw.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://srx.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://pwg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://znn.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://xro.yongpay.top

Go:   // 手写回溯递归
来源：http://nqm.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://vyv.zhengqikj.top

C#:   // 手写回溯递归
来源：http://hrl.zdbjq.cn

[N09] 栈与队列
来源：http://xkx.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zqx.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://avo.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dqh.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xey.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eqz.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kib.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://npd.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vki.daxiang520.top

[N10] 链表节点定义
来源：http://xzg.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qzz.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lqd.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mdq.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vkv.tarul.cn

Java: class Node { int v; Node next; }
来源：http://end.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://sua.hesvh.cn


<!-- 参考信息 -->