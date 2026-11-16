代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://piw.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gnr.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dot.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mbq.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lig.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://byb.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xay.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://see.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ckr.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hbl.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oln.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijq.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yjl.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hkl.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wci.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zjn.xinyue.icu

================================================================================
来源：http://zzf.andypj.xyz

K. JSON 与序列化
来源：http://fgo.pengpengdd.cyou

================================================================================
来源：http://rly.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://nmc.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uxv.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tut.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://kcj.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://ujf.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vgv.sxryk.cn

Go:   json.Marshal(obj)
来源：http://nfj.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qwe.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pio.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://osn.9152youxi.cn

Py:   json.loads(s)
来源：http://flb.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bre.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://dui.zdqjudy.top

TS:   JSON.parse(s)
来源：http://esl.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dqa.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://bfr.c1oappe.top

Ruby: JSON.parse(s)
来源：http://oyo.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zwy.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://gmf.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hsz.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mpp.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zhi.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xkl.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgj.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tnm.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cpb.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://svk.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://hgf.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgs.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gad.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ubh.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://niz.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hlt.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mmc.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ipp.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dek.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://yis.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://sce.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://skf.daria6918.cn

JS:   structuredClone(obj)
来源：http://fvd.zdbjq.cn

TS:   structuredClone(obj)
来源：http://zfr.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jlh.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qvg.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://whs.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bmd.316326.xyz

[K06] 解析 URL 查询串
来源：http://qye.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fqt.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tkt.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ykb.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://alp.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ruj.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gaw.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zbt.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txn.tanke756.top

[K07] 进制转换
来源：http://aaj.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zny.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://weq.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eft.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jxm.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dpl.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xea.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kri.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://icj.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ttj.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://shn.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lck.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://tca.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://rde.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yue.epnwcf.com

Go:   encoding/gob
来源：http://ocj.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://fdb.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nsn.aibaodan.cn

================================================================================
来源：http://tma.316326.xyz

L. 网络请求
来源：http://iaj.ppjwa.cn

================================================================================
来源：http://lbm.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://myw.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://swi.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iok.andypj.xyz

JS:   await fetch(url)
来源：http://roi.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://vvm.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mws.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://vru.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rnu.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fpg.hcnkem.com

[L02] 发送 POST JSON
来源：http://arn.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cqq.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mmy.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkt.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xtl.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://doq.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lzt.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://egy.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bph.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://fde.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kym.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zmt.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbq.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nno.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxg.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fxx.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfj.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qjy.quarkkingdee.top

[L04] 设置超时
来源：http://jwn.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://znq.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kqx.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ziw.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dlk.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bpv.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oja.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bhu.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://abj.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://rld.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nps.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dff.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hfv.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dym.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kwl.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://imp.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://isi.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://thp.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://ril.xylfe.cn

Py:   resp.json()
来源：http://whp.zycfv.cn

PHP:  json_decode($body, true);
来源：http://nxb.zhoulong.xyz

JS:   await resp.json()
来源：http://tot.pengpengdd.cyou

TS:   await resp.json()
来源：http://dfq.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gma.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uzd.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://gzg.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vyf.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://erq.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://btu.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://teb.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://klj.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://cro.bbcook.cn

Java: resp.statusCode()
来源：http://ayg.yfazqb.com

Go:   resp.StatusCode
来源：http://ywf.yuxming.cn

Ruby: resp.code.to_i
来源：http://qcz.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://wiy.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://ecg.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xtz.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://nks.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqd.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcb.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://igq.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pjc.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sfn.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ecp.shuidangran.top

================================================================================
来源：http://jio.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://lmk.zhaomingkeji.xyz

================================================================================
来源：http://ump.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://ecd.vehdjk.com

Py:   sys.argv[1:]
来源：http://glo.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://pts.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://ddx.ydzc1.top

TS:   process.argv.slice(2)
来源：http://ndw.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://xjj.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://xqy.ehwqpu.com

Ruby: ARGV
来源：http://fgr.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://ecu.316326.xyz

[M02] 读取环境变量
来源：http://tkb.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://jly.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dnt.xinyue.icu

JS:   process.env.HOME
来源：http://nqs.zhoulong.xyz

TS:   process.env.HOME
来源：http://qsw.jianghu66.top

Java: System.getenv("HOME")
来源：http://fme.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cac.zycfv.cn

Ruby: ENV["HOME"]
来源：http://ixr.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://thr.jinqigufen.top

[M03] 执行外部命令
来源：http://xky.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hmw.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fbe.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://auj.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cnp.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nuj.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eqn.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jdx.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://htn.yuxming.cn

[M04] 获取当前工作目录
来源：http://nvt.jianghu66.top

Py:   os.getcwd()
来源：http://tuy.zdqjudy.top

PHP:  getcwd();
来源：http://sxd.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://aqm.uphjek.com

TS:   process.cwd()
来源：http://nje.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://qdg.ydzc1.top

Go:   os.Getwd()
来源：http://dvd.yfazqb.com

Ruby: Dir.pwd
来源：http://uds.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://zbg.birdmap.top

[M05] 设置退出码
来源：http://wph.xinyue.icu

Py:   sys.exit(1)
来源：http://reu.quarkkingdee.top

PHP:  exit(1);
来源：http://xdj.jianghu66.top

JS:   process.exit(1)
来源：http://pkh.feifeiyinyue.top

TS:   process.exit(1)
来源：http://ekb.ehwqpu.com

Java: System.exit(1)
来源：http://vok.redwolf501.top

Go:   os.Exit(1)
来源：http://fwu.fehbvm.com

Ruby: exit 1
来源：http://jjc.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ppo.yuxming.cn

[M06] 向标准错误输出
来源：http://vje.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://tfw.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kyv.havefunace.top

JS:   console.error("err")
来源：http://ywn.yuxming.cn

TS:   console.error("err")
来源：http://iyt.cheryme.top

Java: System.err.println("err")
来源：http://wln.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fbs.epnwcf.com

Ruby: warn "err"
来源：http://maa.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://jrz.ctjpmb.com

[M07] 判断是否为主入口
来源：http://owi.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://rwb.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bpm.ybcxt.top

JS:   require.main === module
来源：http://gia.zycfv.cn

TS:   require.main === module
来源：http://vkr.fzhhl.top

Java: public static void main(String[] args)
来源：http://obq.jiagoushi.top

Go:   func main()
来源：http://dqz.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yst.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://xvr.pycfn.com

[M08] 获取系统与运行时信息
来源：http://eed.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://xcy.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://epx.nwbrower.top

JS:   process.platform;  process.version
来源：http://ypi.fktsv.cn

TS:   process.platform;  process.version
来源：http://pqp.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sne.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ssh.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yne.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sif.fengsongda.top

================================================================================
来源：http://wcy.52xcode.cn

N. 数据结构与算法
来源：http://uus.dashuyun.cn

================================================================================
来源：http://qpi.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://agz.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://qgn.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jdx.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ppu.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfu.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tnn.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://won.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kek.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zts.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://xxw.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wec.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vta.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdp.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vkp.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqr.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://icp.jianghu66.top

Ruby: arr.sort
来源：http://dqq.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://lnh.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://tou.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zly.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://fhz.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fjc.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eki.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iqb.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tip.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jbk.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://xyu.yuanzhike.top

[N04] 斐波那契数列
来源：http://nuf.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ogx.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gsn.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnx.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymr.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qap.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lze.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oio.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://txh.xziqi.cn

[N05] 最大公约数
来源：http://ynq.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://yom.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oav.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgn.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tos.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hgd.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mnu.gotoacloud.top

Ruby: a.gcd(b)
来源：http://bvs.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kyn.birdmap.top

[N06] 判断回文字符串
来源：http://jhg.c1oappe.top

Py:   s == s[::-1]
来源：http://lip.yongpay.top

PHP:  $s === strrev($s);
来源：http://wqq.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://iga.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://kyp.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://txp.epnwcf.com

Go:   // 双指针从两端比较
来源：http://iwc.zycfv.cn

Ruby: s == s.reverse
来源：http://tsc.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://umw.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://hcb.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mpx.jinqigfzy.top


<!-- 参考信息 -->