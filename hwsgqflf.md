代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rzd.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://ssb.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tjy.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://ewi.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://few.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dcx.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vsu.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dan.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dyw.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rxq.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pdd.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tev.hnxiangtu.top

================================================================================
来源：http://gpj.kuanghao11.cn

K. JSON 与序列化
来源：http://uut.xingfuxueyuan.xyz

================================================================================
来源：http://sww.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://sde.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mbd.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://scw.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://gxq.sweek.top

TS:   JSON.stringify(obj)
来源：http://ehi.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lug.tarul.cn

Go:   json.Marshal(obj)
来源：http://olw.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://mvp.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qzb.zycfv.cn

[K02] JSON 字符串转对象
来源：http://wpf.tian-w.cn

Py:   json.loads(s)
来源：http://ykv.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nvv.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://ksu.316326.xyz

TS:   JSON.parse(s)
来源：http://yvs.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nke.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://szo.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://ppy.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jho.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://cno.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gry.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rdc.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sbh.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qww.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fot.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nvz.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://evn.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ido.daria6918.cn

[K04] 读取 JSON 文件
来源：http://uxa.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://imf.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://frm.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vae.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyd.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ufg.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sjz.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xdc.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hib.mhx1999.top

[K05] 深拷贝对象
来源：http://gpj.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://roa.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://lkb.epnwcf.com

JS:   structuredClone(obj)
来源：http://emp.jqgfzy.top

TS:   structuredClone(obj)
来源：http://yep.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aqw.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aew.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fkq.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nya.yvedp.cn

[K06] 解析 URL 查询串
来源：http://bbc.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sbt.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://haf.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gre.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tpt.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hrh.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yjs.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nbh.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyr.meibo888.top

[K07] 进制转换
来源：http://vcx.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kqf.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://enx.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://irr.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jik.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vzo.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ztp.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ilk.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kzw.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://fbg.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://kfa.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vbe.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://lnq.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://rwn.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gmj.guowangkeji.top

Go:   encoding/gob
来源：http://ntb.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://isp.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ess.hnqzz.top

================================================================================
来源：http://krk.wangshuangyany.cn

L. 网络请求
来源：http://xwu.sjlbkw.cn

================================================================================
来源：http://ajo.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://adl.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://upc.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bis.hfpthk.cn

JS:   await fetch(url)
来源：http://chn.gogol.net.cn

TS:   await fetch(url)
来源：http://xha.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yye.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://xpe.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://azw.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wxe.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://hxf.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gsm.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyj.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lln.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyg.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sjh.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rib.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zwi.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wqs.epnwcf.com

[L03] 设置自定义请求头
来源：http://zia.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://trb.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eib.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iws.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iqx.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://whv.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cwm.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hmy.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uxc.aibaodan.cn

[L04] 设置超时
来源：http://vms.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://zqm.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ivi.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bfl.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mpe.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fsm.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ajh.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hmh.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kew.52xcode.cn

[L05] 上传文件（multipart）
来源：http://tvu.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oei.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uio.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnz.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aeu.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dnx.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://csn.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asm.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rut.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://kvf.xylfe.cn

Py:   resp.json()
来源：http://tjj.yj202588.top

PHP:  json_decode($body, true);
来源：http://zlq.shangyingyoupin.top

JS:   await resp.json()
来源：http://rsk.jinghuilouyu.cn

TS:   await resp.json()
来源：http://diu.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://odi.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zsf.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://yql.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zvi.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://kcg.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://puo.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mah.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://pyj.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://lfw.sufxvd.cn

Java: resp.statusCode()
来源：http://nde.dianchejie.cn

Go:   resp.StatusCode
来源：http://spe.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://kjb.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://jop.pycfn.com

[L08] 并发请求多个地址
来源：http://hfu.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://teh.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://lfi.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoq.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://enk.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hii.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vgu.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://boh.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dyg.zycfv.cn

================================================================================
来源：http://xtk.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://mlb.xinyue.icu

================================================================================
来源：http://vcx.wangdashe.top

[M01] 读取命令行参数
来源：http://hkk.fehbvm.com

Py:   sys.argv[1:]
来源：http://tqj.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://bif.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://kth.yj202588.top

TS:   process.argv.slice(2)
来源：http://aft.meibo888.top

Java: args 数组（main 方法参数）
来源：http://bzs.shzxlz.cn

Go:   os.Args[1:]
来源：http://lmt.wangdashe.top

Ruby: ARGV
来源：http://wzb.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://vvs.sjlbkw.cn

[M02] 读取环境变量
来源：http://olz.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://uig.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vpv.bbcook.cn

JS:   process.env.HOME
来源：http://rax.sufxvd.cn

TS:   process.env.HOME
来源：http://nzm.hnqzz.top

Java: System.getenv("HOME")
来源：http://lxg.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gwt.yfazqb.com

Ruby: ENV["HOME"]
来源：http://stp.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://faz.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://hfz.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ezp.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tid.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://szy.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oem.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hkq.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hcb.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://pte.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://dyv.meibo888.top

[M04] 获取当前工作目录
来源：http://qmt.xinyue.icu

Py:   os.getcwd()
来源：http://xwl.hnxiangtu.top

PHP:  getcwd();
来源：http://mkn.sufxvd.cn

JS:   process.cwd()
来源：http://ity.zdqjudy.top

TS:   process.cwd()
来源：http://hgk.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://qiq.cqqwz.cn

Go:   os.Getwd()
来源：http://ytq.zhijiandao.cn

Ruby: Dir.pwd
来源：http://yed.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://nes.pengpengdd.cyou

[M05] 设置退出码
来源：http://ntf.cucudq.cn

Py:   sys.exit(1)
来源：http://ixc.andypj.xyz

PHP:  exit(1);
来源：http://qlr.tanke756.top

JS:   process.exit(1)
来源：http://ull.guowangkeji.top

TS:   process.exit(1)
来源：http://nty.hnqzz.top

Java: System.exit(1)
来源：http://qjd.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://lae.gaohongyu789.top

Ruby: exit 1
来源：http://tby.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cai.shuidangran.top

[M06] 向标准错误输出
来源：http://ezp.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://gim.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ydo.sjlbkw.cn

JS:   console.error("err")
来源：http://mbf.yj20258888.top

TS:   console.error("err")
来源：http://udu.xuanzx.com

Java: System.err.println("err")
来源：http://eoh.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://agg.yonumen.top

Ruby: warn "err"
来源：http://fur.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dco.ydzc1.top

[M07] 判断是否为主入口
来源：http://fmy.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://zla.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kns.gotoacloud.top

JS:   require.main === module
来源：http://ljc.guowangkeji.top

TS:   require.main === module
来源：http://dbg.yj20258.top

Java: public static void main(String[] args)
来源：http://xfb.ctjpmb.com

Go:   func main()
来源：http://tjs.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ouk.sweek.top

C#:   static void Main(string[] args)
来源：http://ahe.meibo888.top

[M08] 获取系统与运行时信息
来源：http://cgf.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://ygu.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://qaf.cheryme.top

JS:   process.platform;  process.version
来源：http://jnt.ctjpmb.com

TS:   process.platform;  process.version
来源：http://hne.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qfs.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wlo.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://evf.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://uac.fktsv.cn

================================================================================
来源：http://npe.shzxlz.cn

N. 数据结构与算法
来源：http://pmi.shangyingyoupin.top

================================================================================
来源：http://lvh.yongpay.top

[N01] 二分查找（有序数组）
来源：http://nep.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://kpb.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cow.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlt.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qcl.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kvb.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://dny.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hug.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://qmm.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://csu.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://djf.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tqm.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yut.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bpo.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mmp.xziqi.cn

Go:   slices.Sort(arr)
来源：http://uxp.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://itc.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bqm.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://xnz.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://arj.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://hie.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqv.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tsx.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tau.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fun.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pnv.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://jqd.sufxvd.cn

[N04] 斐波那契数列
来源：http://kuq.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://awg.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qix.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mvu.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lmw.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dlq.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acx.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fht.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rmb.nwbrower.top

[N05] 最大公约数
来源：http://kpb.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://mnl.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lcx.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpg.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dzu.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wlf.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gxx.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://ntm.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fue.hnxiangtu.top

[N06] 判断回文字符串
来源：http://uyb.meibo888.top

Py:   s == s[::-1]
来源：http://rfb.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://rzd.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://mqf.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://xmb.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tns.mhx1999.top

Go:   // 双指针从两端比较
来源：http://tgb.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://zeq.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://dyy.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://byi.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cba.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ihi.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ipt.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://ppx.yvedp.cn

Java: // 手写 HashMap
来源：http://rgk.gaohongyu789.top


<!-- 参考信息 -->