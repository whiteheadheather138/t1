代发 wailian999

[K02] JSON 字符串转对象
来源：http://wuq.haohaochexian.top

Py:   json.loads(s)
来源：http://qlg.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vck.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://uru.xziqi.cn

TS:   JSON.parse(s)
来源：http://kww.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vyc.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://flz.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://wmt.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hhd.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://ogo.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cou.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbf.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ezk.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ycc.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://asf.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://llz.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pzo.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jvi.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://frc.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fho.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aja.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfz.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gje.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://llv.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oqf.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://guc.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pek.gotoacloud.top

[K05] 深拷贝对象
来源：http://ans.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://foe.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://qla.xziqi.cn

JS:   structuredClone(obj)
来源：http://frt.gogol.net.cn

TS:   structuredClone(obj)
来源：http://vjd.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vvq.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pdw.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgr.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://owf.andypj.xyz

[K06] 解析 URL 查询串
来源：http://igy.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lww.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cbc.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ycn.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://siy.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hlw.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hfp.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zpf.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhb.52xcode.cn

[K07] 进制转换
来源：http://zxm.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vqx.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rno.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fmz.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jco.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zdf.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ork.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zcc.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gcu.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://mxe.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://yeu.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cwg.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://tgv.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://mnr.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oot.bbcook.cn

Go:   encoding/gob
来源：http://mle.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://klt.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qpy.cheryme.top

================================================================================
来源：http://tkh.0kj1m.cn

L. 网络请求
来源：http://pme.fktsv.cn

================================================================================
来源：http://iyf.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://mtl.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pwf.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rwl.gotoacloud.top

JS:   await fetch(url)
来源：http://nwt.jqgufenzy.top

TS:   await fetch(url)
来源：http://yos.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfa.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://vmm.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yko.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bxy.tanke756.top

[L02] 发送 POST JSON
来源：http://qby.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://yfk.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hwm.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kju.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tii.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xbo.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wao.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nik.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbt.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://nqb.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pav.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://foc.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://arm.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhl.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ans.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fbc.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fqc.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vps.chenjidiqi.icu

[L04] 设置超时
来源：http://lxh.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://oil.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zkz.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rcy.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xbl.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxo.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uvc.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://chq.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rqn.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://hbz.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dze.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uyn.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://llh.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hzd.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pjg.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqu.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aib.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iht.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://mdv.ctjpmb.com

Py:   resp.json()
来源：http://zlq.xziqi.cn

PHP:  json_decode($body, true);
来源：http://hfo.guannengcc.top

JS:   await resp.json()
来源：http://bcv.fktsv.cn

TS:   await resp.json()
来源：http://cmp.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mjn.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ich.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://vyz.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hwb.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://gub.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://per.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gzb.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://smt.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://ldg.shuidangran.top

Java: resp.statusCode()
来源：http://xkx.jlsjyb.cn

Go:   resp.StatusCode
来源：http://vzc.zhixingplan.top

Ruby: resp.code.to_i
来源：http://nqw.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://ran.jinqigufen.top

[L08] 并发请求多个地址
来源：http://spz.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tlu.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://ffw.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qvp.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gus.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dzc.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zby.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bbr.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fat.shanyushiyangkeji.top

================================================================================
来源：http://hkm.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://mez.zycfv.cn

================================================================================
来源：http://kdf.dashuyun.cn

[M01] 读取命令行参数
来源：http://wjn.snrcjt.cn

Py:   sys.argv[1:]
来源：http://pqy.sysykeji.top

PHP:  $argv;  $argc;
来源：http://uvw.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://pyf.sweek.top

TS:   process.argv.slice(2)
来源：http://law.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://utx.sufxvd.cn

Go:   os.Args[1:]
来源：http://lwv.zhongyouzk.top

Ruby: ARGV
来源：http://unb.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://lhh.cucudq.cn

[M02] 读取环境变量
来源：http://wpt.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://ukm.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iox.jinqigfzy.top

JS:   process.env.HOME
来源：http://qrb.shangyingyoupin.top

TS:   process.env.HOME
来源：http://hlk.zycfv.cn

Java: System.getenv("HOME")
来源：http://kgb.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://duw.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://qml.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cgn.jqgfzy.top

[M03] 执行外部命令
来源：http://gmr.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://svh.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tqu.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mpw.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://ild.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ppd.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wuw.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://dli.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://zec.gogol.net.cn

[M04] 获取当前工作目录
来源：http://jzo.tanke756.top

Py:   os.getcwd()
来源：http://pwl.yuanzhike.top

PHP:  getcwd();
来源：http://mek.fzhhl.top

JS:   process.cwd()
来源：http://bra.snrcjt.cn

TS:   process.cwd()
来源：http://njt.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://pql.jqgufenzy.top

Go:   os.Getwd()
来源：http://iog.sufxvd.cn

Ruby: Dir.pwd
来源：http://nur.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wao.bbcook.cn

[M05] 设置退出码
来源：http://dfj.fengsongda.top

Py:   sys.exit(1)
来源：http://lwa.0kj1m.cn

PHP:  exit(1);
来源：http://nvt.sxryk.cn

JS:   process.exit(1)
来源：http://lam.ybcxt.top

TS:   process.exit(1)
来源：http://dzn.cashguo.top

Java: System.exit(1)
来源：http://xez.yuanzhike.top

Go:   os.Exit(1)
来源：http://dha.daria6918.cn

Ruby: exit 1
来源：http://zbl.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://riv.redwolf501.top

[M06] 向标准错误输出
来源：http://gmh.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://svw.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gyb.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://vsm.guowangkeji.top

TS:   console.error("err")
来源：http://aja.chenzaomai.com

Java: System.err.println("err")
来源：http://xmt.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://myn.xinyue.icu

Ruby: warn "err"
来源：http://mpj.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://rsv.jyoumei.cn

[M07] 判断是否为主入口
来源：http://nhp.birdmap.top

Py:   if __name__ == "__main__":
来源：http://aim.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vzn.shanyushiyangkeji.top

JS:   require.main === module
来源：http://joe.shuidangran.top

TS:   require.main === module
来源：http://nuw.yueranfly.top

Java: public static void main(String[] args)
来源：http://vqh.hammf.cn

Go:   func main()
来源：http://mav.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fin.havefunace.top

C#:   static void Main(string[] args)
来源：http://bxd.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://jiv.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://xka.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://kuz.daria6918.cn

JS:   process.platform;  process.version
来源：http://lvi.yonumen.top

TS:   process.platform;  process.version
来源：http://fqc.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jkr.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uys.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mbw.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uak.gaohongyu789.top

================================================================================
来源：http://jnc.sysykeji.top

N. 数据结构与算法
来源：http://cub.52xcode.cn

================================================================================
来源：http://fvw.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://mzk.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://zrh.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://shy.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://inv.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pxw.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oxa.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://mrt.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hxk.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cht.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://qmr.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ybd.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://afg.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tua.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rdp.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sln.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://wao.chenjidiqi.icu

Ruby: arr.sort
来源：http://jvr.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tja.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://mpv.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zmd.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://qil.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjr.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://epd.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ldr.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uji.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ska.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tzn.yuxming.cn

[N04] 斐波那契数列
来源：http://dtk.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rft.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pha.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eji.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://foc.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ywc.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rpu.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jem.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xqp.ppjwa.cn

[N05] 最大公约数
来源：http://tss.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://dum.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://luf.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://txi.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://igb.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qkk.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nny.ivvv.top

Ruby: a.gcd(b)
来源：http://yma.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rgs.jinqigufen.top

[N06] 判断回文字符串
来源：http://wfm.cdnleiting.top

Py:   s == s[::-1]
来源：http://yic.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://tyc.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://vuk.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://tzv.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eky.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://uri.nanxuanxn.top

Ruby: s == s.reverse
来源：http://clq.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wpl.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://iej.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mxu.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fse.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jyd.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://gfb.gaohongyu789.top

Java: // 手写 HashMap
来源：http://beg.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://kki.sweek.top

Ruby: // 手写 Hash
来源：http://sat.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ceo.bjfxy.top

[N08] 生成全排列
来源：http://god.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://mtg.xinyue.icu

PHP:  // 手写递归交换
来源：http://vtg.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://lzv.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://iue.nanxinkj.top

Java: // 手写回溯递归
来源：http://how.9152youxi.cn

Go:   // 手写回溯递归
来源：http://wlp.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://kby.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://lts.yfazqb.com

[N09] 栈与队列
来源：http://cxq.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cft.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pgk.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kld.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hpe.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pws.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://usc.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cfl.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wob.316326.xyz

[N10] 链表节点定义
来源：http://xnf.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vgw.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://unu.aizwys.cn


<!-- 参考信息 -->