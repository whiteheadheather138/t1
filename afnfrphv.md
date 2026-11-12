代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://czd.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://emh.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iqu.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rya.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tdd.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rmn.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ygr.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qsz.vehdjk.com

================================================================================
来源：http://trb.yongpay.top

K. JSON 与序列化
来源：http://yva.fzhhl.top

================================================================================
来源：http://dib.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://njj.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvs.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fbi.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://rmi.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://pga.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aam.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://oyl.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://xig.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fvb.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://tip.chenjidiqi.icu

Py:   json.loads(s)
来源：http://due.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pax.wangdashe.top

JS:   JSON.parse(s)
来源：http://pcy.guowangkeji.top

TS:   JSON.parse(s)
来源：http://gvb.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cco.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://gsw.redwolf501.top

Ruby: JSON.parse(s)
来源：http://xca.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://akz.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://xks.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cpn.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vhg.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kxw.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ofe.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ktd.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gat.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://tmw.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gzd.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://gvx.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hcp.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sqj.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gtn.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://psv.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://reb.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://enz.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kpu.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dse.ppjwa.cn

[K05] 深拷贝对象
来源：http://hpt.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://yyc.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://rkn.chenzaomai.com

JS:   structuredClone(obj)
来源：http://uyk.xinyue.icu

TS:   structuredClone(obj)
来源：http://ljf.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mpy.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dnp.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsq.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jvi.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://gba.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vaw.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zdj.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vis.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fju.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zgi.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://sla.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tqs.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lsl.tarul.cn

[K07] 进制转换
来源：http://xot.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ohh.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oer.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://syd.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sov.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cxy.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zmf.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ocj.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xkh.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://sbd.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://smw.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://vzx.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://zrp.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://qeh.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tsa.ctjpmb.com

Go:   encoding/gob
来源：http://cfp.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://uec.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fpr.zhaomingkeji.xyz

================================================================================
来源：http://qxy.ehwqpu.com

L. 网络请求
来源：http://hlq.hcnkem.com

================================================================================
来源：http://fmt.cashguo.top

[L01] 发送 GET 请求
来源：http://ilg.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vwf.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gzf.vehdjk.com

JS:   await fetch(url)
来源：http://pct.nwbrower.top

TS:   await fetch(url)
来源：http://wrj.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hfu.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://jut.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cea.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qsl.0kj1m.cn

[L02] 发送 POST JSON
来源：http://jne.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://mka.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ifg.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffy.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbq.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://esy.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dwx.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xec.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ouu.yuxming.cn

[L03] 设置自定义请求头
来源：http://xeu.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lal.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ytu.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mar.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfa.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://flx.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jod.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ioy.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zir.zhijiandao.cn

[L04] 设置超时
来源：http://pks.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://gsf.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://snc.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wop.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhe.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hci.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jii.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mcf.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tey.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://syg.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vzc.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aws.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zdi.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yzw.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://afs.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eqm.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kgq.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gfs.hcnkem.com

[L06] 解析响应为 JSON
来源：http://zno.c1oappe.top

Py:   resp.json()
来源：http://ivm.birdmap.top

PHP:  json_decode($body, true);
来源：http://fwx.jianghu66.top

JS:   await resp.json()
来源：http://jal.yongpay.top

TS:   await resp.json()
来源：http://epk.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xuw.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ljd.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://rln.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lqe.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://kul.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yjg.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ssy.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://byi.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://ory.fehbvm.com

Java: resp.statusCode()
来源：http://xcl.xinyue.icu

Go:   resp.StatusCode
来源：http://pkf.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://vgk.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://prq.haohaochexian.top

[L08] 并发请求多个地址
来源：http://lhv.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zpo.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://wcf.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lrf.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zrn.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bvq.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zhq.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gse.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nwv.yonumen.top

================================================================================
来源：http://rvj.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://mgo.fanxiaobao.xyz

================================================================================
来源：http://jaq.hnxiangtu.top

[M01] 读取命令行参数
来源：http://qsr.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://wkr.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://bnp.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://wqh.havefunace.top

TS:   process.argv.slice(2)
来源：http://roj.sweek.top

Java: args 数组（main 方法参数）
来源：http://ncz.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://idz.nanxuanxn.top

Ruby: ARGV
来源：http://yxj.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://gml.gotoacloud.top

[M02] 读取环境变量
来源：http://twa.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://ekf.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fai.iojbl.cn

JS:   process.env.HOME
来源：http://rzr.daxiang520.top

TS:   process.env.HOME
来源：http://yfa.wangdashe.top

Java: System.getenv("HOME")
来源：http://qyl.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://usn.yueranfly.top

Ruby: ENV["HOME"]
来源：http://fth.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jwn.zycfv.cn

[M03] 执行外部命令
来源：http://gmx.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://byg.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://irq.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sdn.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yym.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mak.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nlw.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://ekv.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://bdu.hysaishi.cn

[M04] 获取当前工作目录
来源：http://byw.xinyue.icu

Py:   os.getcwd()
来源：http://qhr.pycfn.com

PHP:  getcwd();
来源：http://dwe.jiagoushi.top

JS:   process.cwd()
来源：http://ggy.nanxinkj.top

TS:   process.cwd()
来源：http://ygi.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://rdz.yongpay.top

Go:   os.Getwd()
来源：http://zut.vqdsnc.cn

Ruby: Dir.pwd
来源：http://znw.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qhm.feifeiyinyue.top

[M05] 设置退出码
来源：http://cqa.hysaishi.cn

Py:   sys.exit(1)
来源：http://vgs.iojbl.cn

PHP:  exit(1);
来源：http://myp.jqgufenzy.top

JS:   process.exit(1)
来源：http://giu.ppjwa.cn

TS:   process.exit(1)
来源：http://kxz.bjfxy.top

Java: System.exit(1)
来源：http://xck.zycfv.cn

Go:   os.Exit(1)
来源：http://hvh.yj20258.top

Ruby: exit 1
来源：http://hui.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://shv.ydzc1.top

[M06] 向标准错误输出
来源：http://nnk.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://cka.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://auz.bjfxy.top

JS:   console.error("err")
来源：http://hec.svipenyu.cn

TS:   console.error("err")
来源：http://chf.hywenlv.cn

Java: System.err.println("err")
来源：http://bua.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqn.jiagoushi.top

Ruby: warn "err"
来源：http://yco.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://zsf.yuxming.cn

[M07] 判断是否为主入口
来源：http://skf.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://kcn.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lrf.guowangkeji.top

JS:   require.main === module
来源：http://tmh.bbcook.cn

TS:   require.main === module
来源：http://czf.daria6918.cn

Java: public static void main(String[] args)
来源：http://ehc.yuanzhike.top

Go:   func main()
来源：http://pnq.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cvf.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://som.ivvv.top

[M08] 获取系统与运行时信息
来源：http://gqx.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://fin.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://gdf.316326.xyz

JS:   process.platform;  process.version
来源：http://iix.daria6918.cn

TS:   process.platform;  process.version
来源：http://rcq.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://myl.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oze.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ybl.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cfo.yueranfly.top

================================================================================
来源：http://uzm.iojbl.cn

N. 数据结构与算法
来源：http://mvy.ivvv.top

================================================================================
来源：http://rby.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://qji.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://uqx.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dwe.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpc.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixr.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://nyf.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ynp.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zle.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://vzd.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://ftv.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://tbc.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cww.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://doz.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hek.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://grv.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://ncg.yj202588.top

Ruby: arr.sort
来源：http://yvu.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://njw.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://tqk.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xbh.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://jqv.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fql.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otd.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bzf.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://myr.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oes.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://esy.wangdashe.top

[N04] 斐波那契数列
来源：http://snr.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jgb.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oud.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xcc.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wyw.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lsq.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hyh.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://axn.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hmr.yj20258.top

[N05] 最大公约数
来源：http://cuq.cheryme.top

Py:   math.gcd(a, b)
来源：http://est.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pka.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovl.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://psx.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kec.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vyp.sufxvd.cn

Ruby: a.gcd(b)
来源：http://zsa.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsm.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://hep.shuidangran.top

Py:   s == s[::-1]
来源：http://rei.xylfe.cn

PHP:  $s === strrev($s);
来源：http://sbl.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://anc.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://pol.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jjq.redwolf501.top

Go:   // 双指针从两端比较
来源：http://cnc.hcnkem.com

Ruby: s == s.reverse
来源：http://eda.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xfe.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://oqr.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://skq.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ney.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://avm.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://vav.yvedp.cn

Java: // 手写 HashMap
来源：http://dvo.aizwys.cn

Go:   // 手写 map[int]int
来源：http://prl.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://hec.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://fbn.jyoumei.cn

[N08] 生成全排列
来源：http://bmb.zhixingplan.top


<!-- 参考信息 -->