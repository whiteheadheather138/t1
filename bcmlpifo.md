代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ytd.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ehi.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vyu.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://lcv.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tmn.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rrz.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yil.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ngu.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yhs.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gqb.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqf.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iqw.zhiwuduotai.top

================================================================================
来源：http://rgi.shangyingyoupin.top

K. JSON 与序列化
来源：http://wwq.quarkkingdee.top

================================================================================
来源：http://uvs.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://wva.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkx.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ovy.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://rbi.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://ved.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oau.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://fyb.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ndv.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://uqx.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://mke.hnxiangtu.top

Py:   json.loads(s)
来源：http://rvp.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vya.52xcode.cn

JS:   JSON.parse(s)
来源：http://yvg.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://pmb.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ppx.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://wsm.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://fmq.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://agr.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://erk.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kco.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jkr.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://coq.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fis.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ikc.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xrh.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dtx.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tix.bbcook.cn

[K04] 读取 JSON 文件
来源：http://bav.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kur.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nmp.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhr.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aoj.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rcd.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xec.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wmi.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ebm.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://erj.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://lpc.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://tdb.cqqwz.cn

JS:   structuredClone(obj)
来源：http://rqc.yfazqb.com

TS:   structuredClone(obj)
来源：http://gxs.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://drs.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://msx.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zym.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://pfq.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://rxz.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vgz.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vqj.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewp.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjp.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tqr.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://orb.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://abt.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://frc.jianghu66.top

[K07] 进制转换
来源：http://dxy.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kgy.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pgj.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hvv.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://phv.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znt.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://szi.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hjb.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ddp.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://ekz.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://oyd.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ayh.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://jse.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://zoz.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gjv.shuidangran.top

Go:   encoding/gob
来源：http://cos.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://ytd.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qtt.zhiwuduotai.top

================================================================================
来源：http://ufo.jinqigfzy.top

L. 网络请求
来源：http://gwt.chenjidiqi.icu

================================================================================
来源：http://yms.hfpthk.cn

[L01] 发送 GET 请求
来源：http://buj.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qmd.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sow.yfazqb.com

JS:   await fetch(url)
来源：http://kel.yanxiufei.cn

TS:   await fetch(url)
来源：http://rnv.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmj.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://dkh.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://afi.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nad.pycfn.com

[L02] 发送 POST JSON
来源：http://hnf.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lke.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vym.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vvw.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zss.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vza.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://orv.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wwm.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ilx.dianchejie.cn

[L03] 设置自定义请求头
来源：http://kis.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dop.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uxs.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://etc.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bnw.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yoe.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xjk.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pih.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hpb.yueranfly.top

[L04] 设置超时
来源：http://hnf.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://hrx.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvk.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ans.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmb.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://udm.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uat.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eul.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dar.jianghu66.top

[L05] 上传文件（multipart）
来源：http://cqs.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://szd.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lyt.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hjl.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zek.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kda.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rxi.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uez.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ofb.hcnkem.com

[L06] 解析响应为 JSON
来源：http://lgu.cashguo.top

Py:   resp.json()
来源：http://qqq.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://bow.cdnleiting.top

JS:   await resp.json()
来源：http://gbx.hywenlv.cn

TS:   await resp.json()
来源：http://fny.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://amw.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gxq.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://xcd.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dyl.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://kpv.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qad.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xoo.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://ttr.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://dnx.jqgufenzy.top

Java: resp.statusCode()
来源：http://ewp.gzhubu.top

Go:   resp.StatusCode
来源：http://gva.xziqi.cn

Ruby: resp.code.to_i
来源：http://lxg.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://mkx.ehwqpu.com

[L08] 并发请求多个地址
来源：http://aaa.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://smj.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://ywc.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ops.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsl.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rik.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zcy.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kgy.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vbm.fanxiaobao.xyz

================================================================================
来源：http://jsw.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://ngq.yuanzhike.top

================================================================================
来源：http://fnn.sjlbkw.cn

[M01] 读取命令行参数
来源：http://vea.guannengcc.top

Py:   sys.argv[1:]
来源：http://kve.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://ase.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://udz.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://xto.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://oyv.nanxuanxn.top

Go:   os.Args[1:]
来源：http://vyk.cashguo.top

Ruby: ARGV
来源：http://jby.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://liw.jinqigufen.top

[M02] 读取环境变量
来源：http://eqh.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://bnz.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jzb.jqgfzy.top

JS:   process.env.HOME
来源：http://eqk.gaohongyu789.top

TS:   process.env.HOME
来源：http://yce.yvedp.cn

Java: System.getenv("HOME")
来源：http://znk.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://biu.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://yln.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kte.ydzc1.top

[M03] 执行外部命令
来源：http://pai.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rim.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sav.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vyw.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ggs.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rje.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vki.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://fnu.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://hzh.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://dfx.ybcxt.top

Py:   os.getcwd()
来源：http://rnw.9152youxi.cn

PHP:  getcwd();
来源：http://cgg.yfazqb.com

JS:   process.cwd()
来源：http://mlx.aibaodan.cn

TS:   process.cwd()
来源：http://jye.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://qmy.xinyue.icu

Go:   os.Getwd()
来源：http://nno.smart0.xyz

Ruby: Dir.pwd
来源：http://auo.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://jfx.yangfankeji.com

[M05] 设置退出码
来源：http://rcx.bbcook.cn

Py:   sys.exit(1)
来源：http://sfo.jiagoushi.top

PHP:  exit(1);
来源：http://fsr.52xcode.cn

JS:   process.exit(1)
来源：http://beh.ydzc1.top

TS:   process.exit(1)
来源：http://iby.jlsjyb.cn

Java: System.exit(1)
来源：http://dfj.pycfn.com

Go:   os.Exit(1)
来源：http://stg.cqqwz.cn

Ruby: exit 1
来源：http://vpy.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://djk.aizwys.cn

[M06] 向标准错误输出
来源：http://rkq.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://msg.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xjn.shangyingyoupin.top

JS:   console.error("err")
来源：http://gck.yonumen.top

TS:   console.error("err")
来源：http://wak.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://oje.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iun.feifeiyinyue.top

Ruby: warn "err"
来源：http://tao.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://zik.hywenlv.cn

[M07] 判断是否为主入口
来源：http://hgk.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://kpv.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wlm.cheryme.top

JS:   require.main === module
来源：http://ggz.zhijiandao.cn

TS:   require.main === module
来源：http://nrv.xziqi.cn

Java: public static void main(String[] args)
来源：http://efg.fengsongda.top

Go:   func main()
来源：http://ser.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hzc.sysykeji.top

C#:   static void Main(string[] args)
来源：http://odl.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://jwi.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://zyf.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://gdx.ybcxt.top

JS:   process.platform;  process.version
来源：http://pyb.xziqi.cn

TS:   process.platform;  process.version
来源：http://mrx.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mbg.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hij.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qlj.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lqc.zycfv.cn

================================================================================
来源：http://tdc.aibaodan.cn

N. 数据结构与算法
来源：http://ssx.jqgufenzy.top

================================================================================
来源：http://hwa.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://ehw.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fvc.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyu.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hrk.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcj.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://glp.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://ssv.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xel.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://dqo.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://iwf.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://tzs.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gdp.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://frx.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://efq.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jbq.xuanzx.com

Go:   slices.Sort(arr)
来源：http://uup.c1oappe.top

Ruby: arr.sort
来源：http://zbu.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jfe.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://lsj.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rtf.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://zdo.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ajn.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mzm.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wsx.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gel.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wza.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://auc.redwolf501.top

[N04] 斐波那契数列
来源：http://ubl.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sor.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wko.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfb.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zif.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bvn.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://shf.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://neg.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uge.yonumen.top

[N05] 最大公约数
来源：http://pgy.wangdashe.top

Py:   math.gcd(a, b)
来源：http://npi.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rqh.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jon.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idw.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dfn.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wau.hammf.cn

Ruby: a.gcd(b)
来源：http://fqn.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xpc.zhixingplan.top

[N06] 判断回文字符串
来源：http://nrz.iojbl.cn

Py:   s == s[::-1]
来源：http://wni.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://iqb.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://nhx.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://lnh.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfk.yfazqb.com

Go:   // 双指针从两端比较
来源：http://tag.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://mhs.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://euj.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://mon.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ztl.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xyt.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://trb.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://kxr.0kj1m.cn

Java: // 手写 HashMap
来源：http://wms.hnxiangtu.top


<!-- 参考信息 -->