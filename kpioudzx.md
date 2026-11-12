代发 wailian999

TS:   JSON.parse(s)
来源：http://rmf.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hje.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://mjc.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://pad.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://csj.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://mek.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ohn.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fts.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ahp.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rrr.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xeh.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qjk.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fyk.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qrr.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://ogn.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yap.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vmx.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rnh.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcq.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vsm.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ygy.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qby.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ere.epnwcf.com

[K05] 深拷贝对象
来源：http://hsc.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://ynw.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://vbe.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://coj.gotoacloud.top

TS:   structuredClone(obj)
来源：http://sjo.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yds.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jkx.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkw.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xez.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://yms.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://awt.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bcx.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwj.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgp.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hid.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ndx.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dvu.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uiu.fehbvm.com

[K07] 进制转换
来源：http://hfv.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ows.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yim.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jkn.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lnm.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://afu.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://plc.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sdy.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cfy.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://kic.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://kyw.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mak.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://hgm.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://jjm.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ogh.shuidangran.top

Go:   encoding/gob
来源：http://nsz.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://aoz.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cch.jinqigfzy.top

================================================================================
来源：http://wte.xziqi.cn

L. 网络请求
来源：http://bvm.ppjwa.cn

================================================================================
来源：http://tna.xylfe.cn

[L01] 发送 GET 请求
来源：http://ytg.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://evo.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ufj.hongshengwenyu.top

JS:   await fetch(url)
来源：http://bnl.sjlbkw.cn

TS:   await fetch(url)
来源：http://hjp.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://apq.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://bhq.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fed.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uyb.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://pwl.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jui.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kxd.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ehy.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ncj.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wxm.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://akl.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cll.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ofh.meibo888.top

[L03] 设置自定义请求头
来源：http://wnx.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kzp.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bms.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gyo.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dds.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ryp.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ubv.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://udd.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zrr.meibo888.top

[L04] 设置超时
来源：http://tci.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://kml.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bpc.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sfk.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzr.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wzl.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nud.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ybn.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xwm.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://sqm.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cqd.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wyw.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cey.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qxe.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ugy.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://epj.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cub.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tnq.yfazqb.com

[L06] 解析响应为 JSON
来源：http://cbg.zhaomingkeji.xyz

Py:   resp.json()
来源：http://rvr.cashguo.top

PHP:  json_decode($body, true);
来源：http://hpg.bbcook.cn

JS:   await resp.json()
来源：http://qux.zhongyouzk.top

TS:   await resp.json()
来源：http://mhm.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vrc.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cpv.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://jwa.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iui.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://hef.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jlk.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yuh.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://zvo.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://dru.birdmap.top

Java: resp.statusCode()
来源：http://jrl.ctjpmb.com

Go:   resp.StatusCode
来源：http://haq.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://yim.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://cva.hammf.cn

[L08] 并发请求多个地址
来源：http://iag.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ois.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://cpx.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfx.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pnt.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hzq.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zjv.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://taf.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sow.bjfxy.top

================================================================================
来源：http://sab.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://sgj.sweek.top

================================================================================
来源：http://iso.mhx1999.top

[M01] 读取命令行参数
来源：http://ymu.haohaochexian.top

Py:   sys.argv[1:]
来源：http://bnh.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://mas.gzhubu.top

JS:   process.argv.slice(2)
来源：http://dzs.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://zaj.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://rya.nanxinkj.top

Go:   os.Args[1:]
来源：http://ecp.ywan-chungtsiang.top

Ruby: ARGV
来源：http://gdi.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://hav.yueranfly.top

[M02] 读取环境变量
来源：http://vti.meibo888.top

Py:   os.environ.get("HOME")
来源：http://vss.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mpy.bjfxy.top

JS:   process.env.HOME
来源：http://mdw.haohaochexian.top

TS:   process.env.HOME
来源：http://sbk.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://wgb.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mpe.yuxming.cn

Ruby: ENV["HOME"]
来源：http://ozb.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dnc.zhongyouzk.top

[M03] 执行外部命令
来源：http://mgn.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oxd.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dqw.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://aur.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://txk.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gsz.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hci.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://olb.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://rcp.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://duf.smart0.xyz

Py:   os.getcwd()
来源：http://lvk.fehbvm.com

PHP:  getcwd();
来源：http://oek.shangyingyoupin.top

JS:   process.cwd()
来源：http://cfw.daxiang520.top

TS:   process.cwd()
来源：http://vnu.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://fkq.zhoulong.xyz

Go:   os.Getwd()
来源：http://lmm.vqdsnc.cn

Ruby: Dir.pwd
来源：http://daa.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://lgq.yangfankeji.com

[M05] 设置退出码
来源：http://oox.yj20258888.top

Py:   sys.exit(1)
来源：http://zyg.sxryk.cn

PHP:  exit(1);
来源：http://qzw.9152youxi.cn

JS:   process.exit(1)
来源：http://fya.hesvh.cn

TS:   process.exit(1)
来源：http://twq.ctjpmb.com

Java: System.exit(1)
来源：http://qov.hcnkem.com

Go:   os.Exit(1)
来源：http://gus.mhx1999.top

Ruby: exit 1
来源：http://erg.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxx.hysaishi.cn

[M06] 向标准错误输出
来源：http://nnk.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://gnk.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://met.jqgufenzy.top

JS:   console.error("err")
来源：http://wid.fzhhl.top

TS:   console.error("err")
来源：http://jiw.chenzaomai.com

Java: System.err.println("err")
来源：http://yza.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fjl.xuetiantiany.cn

Ruby: warn "err"
来源：http://spx.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://mdd.hcnkem.com

[M07] 判断是否为主入口
来源：http://nte.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://bln.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rjv.kuanghao11.cn

JS:   require.main === module
来源：http://xwo.cdnleiting.top

TS:   require.main === module
来源：http://ofk.yvedp.cn

Java: public static void main(String[] args)
来源：http://akz.ctjpmb.com

Go:   func main()
来源：http://xqn.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://chd.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://qyr.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://ujg.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://zvi.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://dco.hammf.cn

JS:   process.platform;  process.version
来源：http://pbi.yuxming.cn

TS:   process.platform;  process.version
来源：http://mga.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://krl.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://qxf.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://flb.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lmj.gaohongyu789.top

================================================================================
来源：http://vja.ctjpmb.com

N. 数据结构与算法
来源：http://ewt.hysaishi.cn

================================================================================
来源：http://cuq.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://iol.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ira.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ljo.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgm.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://etc.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://yaf.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://bay.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://kfm.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://ktt.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://lnb.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://pqx.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jdp.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dsn.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mgl.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sdl.ybcxt.top

Go:   slices.Sort(arr)
来源：http://lkl.vehdjk.com

Ruby: arr.sort
来源：http://slh.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://epw.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://ssr.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zuz.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://ngb.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tkz.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oop.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pdd.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://meu.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dfb.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://yeu.cheryme.top

[N04] 斐波那契数列
来源：http://cpz.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uen.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://asp.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yuu.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yug.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbt.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zdg.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bob.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fld.zhiwuduotai.top

[N05] 最大公约数
来源：http://lgr.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://qcv.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://elr.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgr.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkx.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ubj.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yjh.hfpthk.cn

Ruby: a.gcd(b)
来源：http://cbe.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kry.zdbjq.cn

[N06] 判断回文字符串
来源：http://pjt.redwolf501.top

Py:   s == s[::-1]
来源：http://woj.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://bzj.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://wov.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://wni.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lof.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://qoo.uphjek.com

Ruby: s == s.reverse
来源：http://ssk.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://mbw.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://swk.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ieu.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lvh.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oir.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://wpt.9152youxi.cn

Java: // 手写 HashMap
来源：http://yrl.iojbl.cn

Go:   // 手写 map[int]int
来源：http://lwf.guannengcc.top

Ruby: // 手写 Hash
来源：http://dzg.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gcm.pycfn.com

[N08] 生成全排列
来源：http://gtn.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://shx.bjfxy.top

PHP:  // 手写递归交换
来源：http://dmj.redwolf501.top

JS:   // 手写回溯递归
来源：http://wmc.hnqzz.top

TS:   // 手写回溯递归
来源：http://hex.hesvh.cn

Java: // 手写回溯递归
来源：http://hse.yuanzhike.top

Go:   // 手写回溯递归
来源：http://luy.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://rdj.bjfxy.top

C#:   // 手写回溯递归
来源：http://rtj.shzxlz.cn

[N09] 栈与队列
来源：http://omd.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rrp.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fhe.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bpp.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vny.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crj.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aor.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mzf.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://awq.nwbrower.top

[N10] 链表节点定义
来源：http://zcb.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tyx.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tpn.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pum.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fhd.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://xmq.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://jfa.shzxlz.cn


<!-- 参考信息 -->