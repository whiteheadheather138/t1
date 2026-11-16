代发 wailian999

[K02] JSON 字符串转对象
来源：http://typ.zhongyouzk.top

Py:   json.loads(s)
来源：http://drn.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vnx.nanxinkj.top

JS:   JSON.parse(s)
来源：http://qfu.iojbl.cn

TS:   JSON.parse(s)
来源：http://vxi.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uqy.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://tyj.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://vwz.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://alx.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://trz.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gck.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://isa.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vuj.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ndp.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bbr.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yxy.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://pou.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhi.ydzc1.top

[K04] 读取 JSON 文件
来源：http://hts.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgy.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wbp.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://obn.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xcl.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sji.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lno.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dmk.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ayt.jlsjyb.cn

[K05] 深拷贝对象
来源：http://rth.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://buq.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://hme.zhixingplan.top

JS:   structuredClone(obj)
来源：http://ltb.cucudq.cn

TS:   structuredClone(obj)
来源：http://wpg.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://liw.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aay.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bkq.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://exg.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://hjo.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hkf.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oec.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://soq.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oib.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://doy.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aho.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ari.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dpw.jinghuilouyu.cn

[K07] 进制转换
来源：http://ucj.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mgz.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lgy.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yed.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ahp.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jty.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://omy.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gko.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xtw.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://xgp.sweek.top

Py:   pickle.dumps(obj)
来源：http://osu.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wkv.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://hka.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://nqu.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hmc.meibo888.top

Go:   encoding/gob
来源：http://wpk.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://zgn.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qth.yongpay.top

================================================================================
来源：http://fmb.mhx1999.top

L. 网络请求
来源：http://ffd.xylfe.cn

================================================================================
来源：http://iwf.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://zxw.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kcg.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tve.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://gwh.pengpengdd.cyou

TS:   await fetch(url)
来源：http://qse.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oce.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://neh.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xuc.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://krq.vehdjk.com

[L02] 发送 POST JSON
来源：http://uwx.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://cmv.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bvu.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzh.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nec.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tew.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jed.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ydt.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhw.gzhubu.top

[L03] 设置自定义请求头
来源：http://aqr.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://axl.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://skz.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydq.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhe.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yqm.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vta.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qox.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ivr.nwbrower.top

[L04] 设置超时
来源：http://kga.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://ecn.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fng.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ess.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://icf.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://shi.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jsn.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://puy.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hhy.fzhhl.top

[L05] 上传文件（multipart）
来源：http://ido.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hmh.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dcf.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ywl.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hth.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmr.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://scw.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yde.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eul.yongpay.top

[L06] 解析响应为 JSON
来源：http://hur.jinghuilouyu.cn

Py:   resp.json()
来源：http://chp.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://wkl.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://tpy.iojbl.cn

TS:   await resp.json()
来源：http://yew.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xcy.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ruy.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://fla.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://myj.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://ntn.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mcb.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://osa.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://vpm.meibo888.top

TS:   resp.ok;  resp.status
来源：http://jpi.yuxming.cn

Java: resp.statusCode()
来源：http://gou.snrcjt.cn

Go:   resp.StatusCode
来源：http://qng.ctjpmb.com

Ruby: resp.code.to_i
来源：http://gnz.hammf.cn

C#:   (int)resp.StatusCode
来源：http://wvm.hfpthk.cn

[L08] 并发请求多个地址
来源：http://nsf.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xxa.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://iqt.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usy.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ptf.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dwj.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pnj.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zjw.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kdq.bbcook.cn

================================================================================
来源：http://ovf.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://wws.shanyushiyangtech.top

================================================================================
来源：http://xjb.vqdsnc.cn

[M01] 读取命令行参数
来源：http://yug.hfpthk.cn

Py:   sys.argv[1:]
来源：http://fti.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://eod.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://pbt.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://vxe.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://owu.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://hbz.chenjidiqi.icu

Ruby: ARGV
来源：http://cyr.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://mgj.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://zdd.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://htu.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ypf.yj20258888.top

JS:   process.env.HOME
来源：http://svf.smart0.xyz

TS:   process.env.HOME
来源：http://oyz.zhixingplan.top

Java: System.getenv("HOME")
来源：http://tbv.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vpl.guannengcc.top

Ruby: ENV["HOME"]
来源：http://lsd.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xwo.yongpay.top

[M03] 执行外部命令
来源：http://izu.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tan.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gkn.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rdw.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qaw.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://beh.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dml.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wjx.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://aud.gzhubu.top

[M04] 获取当前工作目录
来源：http://hal.dashuyun.cn

Py:   os.getcwd()
来源：http://nct.wangshuangyany.cn

PHP:  getcwd();
来源：http://who.tarul.cn

JS:   process.cwd()
来源：http://skv.cucudq.cn

TS:   process.cwd()
来源：http://yrz.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://ztc.316326.xyz

Go:   os.Getwd()
来源：http://gdj.c1oappe.top

Ruby: Dir.pwd
来源：http://bfr.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://xon.zhiwuduotai.top

[M05] 设置退出码
来源：http://moe.zhengqikj.top

Py:   sys.exit(1)
来源：http://btm.wangdashe.top

PHP:  exit(1);
来源：http://avk.pycfn.com

JS:   process.exit(1)
来源：http://qcz.ydzc1.top

TS:   process.exit(1)
来源：http://hhm.hnxiangtu.top

Java: System.exit(1)
来源：http://ccb.gzhubu.top

Go:   os.Exit(1)
来源：http://jfv.jqgufenzy.top

Ruby: exit 1
来源：http://wra.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cif.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://fas.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://ypv.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ryz.meibo888.top

JS:   console.error("err")
来源：http://bkb.xuetiantiany.cn

TS:   console.error("err")
来源：http://hkv.nanxinkj.top

Java: System.err.println("err")
来源：http://lju.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rlj.sjlbkw.cn

Ruby: warn "err"
来源：http://qzi.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://zfk.aibaodan.cn

[M07] 判断是否为主入口
来源：http://tnt.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://wgw.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oxp.ctjpmb.com

JS:   require.main === module
来源：http://jnn.smart0.xyz

TS:   require.main === module
来源：http://vkq.zhengqikj.top

Java: public static void main(String[] args)
来源：http://vjc.mhx1999.top

Go:   func main()
来源：http://hzy.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uwd.daria6918.cn

C#:   static void Main(string[] args)
来源：http://vac.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://sry.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://dvs.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://uaq.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://dbx.yuanzhike.top

TS:   process.platform;  process.version
来源：http://hkz.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jdo.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://doo.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ofl.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nhu.redwolf501.top

================================================================================
来源：http://hqx.havefunace.top

N. 数据结构与算法
来源：http://pjp.daria6918.cn

================================================================================
来源：http://osp.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://byi.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://ume.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nqi.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dbo.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bsl.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yof.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://kbb.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://woc.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://oam.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://nyn.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://voy.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rfw.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ija.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kxp.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://neh.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://but.yj20258888.top

Ruby: arr.sort
来源：http://ofa.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cjo.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://esa.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fmb.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://uqt.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dap.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojn.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eaj.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oes.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sfe.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://axt.xuanzx.com

[N04] 斐波那契数列
来源：http://afb.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvs.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thu.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bmv.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://utm.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ope.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fxm.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xer.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sdr.snrcjt.cn

[N05] 最大公约数
来源：http://cju.aizwys.cn

Py:   math.gcd(a, b)
来源：http://gza.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://crc.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lag.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ucu.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kef.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ies.ctjpmb.com

Ruby: a.gcd(b)
来源：http://qnv.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://suv.c1oappe.top

[N06] 判断回文字符串
来源：http://iai.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://jkv.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://xxd.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://khn.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://xal.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzn.316326.xyz

Go:   // 双指针从两端比较
来源：http://mty.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://vkr.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dax.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://ipo.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jqb.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cgp.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dcc.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://swd.daria6918.cn

Java: // 手写 HashMap
来源：http://clb.yj20258888.top

Go:   // 手写 map[int]int
来源：http://mvf.gogol.net.cn

Ruby: // 手写 Hash
来源：http://tgb.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://hqo.ehwqpu.com

[N08] 生成全排列
来源：http://ezn.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://kif.zhixingplan.top

PHP:  // 手写递归交换
来源：http://qlf.ydzc1.top

JS:   // 手写回溯递归
来源：http://vba.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://mld.jinqigfzy.top

Java: // 手写回溯递归
来源：http://ipw.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://bbr.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://eoe.fzhhl.top

C#:   // 手写回溯递归
来源：http://cme.zhongyouzk.top

[N09] 栈与队列
来源：http://qwv.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wks.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vrp.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hzt.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xrz.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mmn.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zcv.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ihr.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fmb.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://hfo.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nvz.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ypp.yanxiufei.cn


<!-- 参考信息 -->