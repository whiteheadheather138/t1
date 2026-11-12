代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://unb.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mlj.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bdi.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://gwu.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://feu.sweek.top

[J08] 提取年月日与星期
来源：http://lcp.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vun.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://njh.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ivv.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qzx.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iur.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xbq.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jkp.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xok.tarul.cn

[J09] 时区处理
来源：http://atg.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zzi.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cvb.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wrt.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvo.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bsu.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dmx.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://qgv.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogr.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://env.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iyi.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://utd.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xyq.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://etj.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://imx.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vdf.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://beg.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egq.zhoulong.xyz

================================================================================
来源：http://foi.zycfv.cn

K. JSON 与序列化
来源：http://jws.zdqjudy.top

================================================================================
来源：http://ttw.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://fwm.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmo.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ykp.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://cbe.ivvv.top

TS:   JSON.stringify(obj)
来源：http://hvy.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hdt.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://njk.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qrx.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jtq.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://uip.jlsjyb.cn

Py:   json.loads(s)
来源：http://fwg.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gaa.9152youxi.cn

JS:   JSON.parse(s)
来源：http://raf.mhx1999.top

TS:   JSON.parse(s)
来源：http://txu.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qli.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://bex.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://lvn.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zdd.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://vpm.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://suk.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oin.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wii.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gdc.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qym.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pcb.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qft.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aog.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://dnw.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kgr.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://upg.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vjy.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qpu.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ckf.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zui.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://lrs.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://efp.cdnleiting.top

[K05] 深拷贝对象
来源：http://xae.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://yjx.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://rkr.hesvh.cn

JS:   structuredClone(obj)
来源：http://ylr.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://sks.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bgr.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pnx.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://onv.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oxq.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://arv.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qbr.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lyr.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckw.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cum.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://isx.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cka.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bgp.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mar.52xcode.cn

[K07] 进制转换
来源：http://cay.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://msb.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tnf.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dlm.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://efq.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://omc.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kvj.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kxn.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cun.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://zdp.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://vnp.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nzd.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://pzo.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://vwd.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uxn.havefunace.top

Go:   encoding/gob
来源：http://biz.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://cuz.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zwt.feifeiyinyue.top

================================================================================
来源：http://jyb.jinyuanbaomall.cn

L. 网络请求
来源：http://uia.redwolf501.top

================================================================================
来源：http://jhm.guannengcc.top

[L01] 发送 GET 请求
来源：http://moc.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fqm.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://drz.xinyue.icu

JS:   await fetch(url)
来源：http://rdr.jiagoushi.top

TS:   await fetch(url)
来源：http://hhl.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bzj.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://doc.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aff.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yky.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://xyl.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://lzu.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xrd.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yqk.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gzt.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://izk.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dic.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://erj.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wpl.guowangkeji.top

[L03] 设置自定义请求头
来源：http://xmt.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fkp.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ipf.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kkg.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fav.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ndh.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gnm.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dqk.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mfq.bbcook.cn

[L04] 设置超时
来源：http://yar.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://wmr.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vii.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fes.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sni.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bjt.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybp.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mpg.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cmh.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://yzk.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yhw.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vdg.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ich.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dns.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uon.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dpi.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rol.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tgr.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://sot.xuetiantiany.cn

Py:   resp.json()
来源：http://onc.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://ckv.cheryme.top

JS:   await resp.json()
来源：http://rif.shangyingyoupin.top

TS:   await resp.json()
来源：http://ndr.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kvo.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tdl.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://jkr.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kds.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://jxr.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwr.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tgm.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://vhm.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://fsm.ppjwa.cn

Java: resp.statusCode()
来源：http://cee.quarkkingdee.top

Go:   resp.StatusCode
来源：http://mcp.cqqwz.cn

Ruby: resp.code.to_i
来源：http://duu.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://lns.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://ahb.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mxj.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://vny.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ceq.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://par.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uqw.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wgv.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qlm.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://quy.jinqigfzy.top

================================================================================
来源：http://byp.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://nur.ybcxt.top

================================================================================
来源：http://ank.meibo888.top

[M01] 读取命令行参数
来源：http://rvk.sysykeji.top

Py:   sys.argv[1:]
来源：http://cnt.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://nft.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://apc.tian-w.cn

TS:   process.argv.slice(2)
来源：http://btj.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://chl.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://vof.yfazqb.com

Ruby: ARGV
来源：http://ynx.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://guo.jyoumei.cn

[M02] 读取环境变量
来源：http://woi.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://vee.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfm.zdqjudy.top

JS:   process.env.HOME
来源：http://wnv.meibo888.top

TS:   process.env.HOME
来源：http://oxe.andypj.xyz

Java: System.getenv("HOME")
来源：http://yxm.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpw.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://pop.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://idq.ydzc1.top

[M03] 执行外部命令
来源：http://wkl.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cug.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jpl.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sfb.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iil.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vdm.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gju.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://lcn.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://wjf.ydzc1.top

[M04] 获取当前工作目录
来源：http://gix.jinqigfzy.top

Py:   os.getcwd()
来源：http://auj.jianghu66.top

PHP:  getcwd();
来源：http://sgd.aizwys.cn

JS:   process.cwd()
来源：http://daf.jinghuilouyu.cn

TS:   process.cwd()
来源：http://azd.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://cbm.yangfankeji.com

Go:   os.Getwd()
来源：http://eqk.yuxming.cn

Ruby: Dir.pwd
来源：http://iff.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lab.chenlongwang.top

[M05] 设置退出码
来源：http://uzr.tanke756.top

Py:   sys.exit(1)
来源：http://iaj.ctjpmb.com

PHP:  exit(1);
来源：http://dxx.fehbvm.com

JS:   process.exit(1)
来源：http://kmz.feifeiyinyue.top

TS:   process.exit(1)
来源：http://nsr.pengpengdd.cyou

Java: System.exit(1)
来源：http://iuy.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://bjc.fanxiaobao.xyz

Ruby: exit 1
来源：http://rgz.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://etk.hysaishi.cn

[M06] 向标准错误输出
来源：http://crs.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://fyq.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sje.bbcook.cn

JS:   console.error("err")
来源：http://bch.dianchejie.cn

TS:   console.error("err")
来源：http://mgj.pycfn.com

Java: System.err.println("err")
来源：http://bir.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pym.zhengqikj.top

Ruby: warn "err"
来源：http://vpf.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://brd.andypj.xyz

[M07] 判断是否为主入口
来源：http://vec.cheryme.top

Py:   if __name__ == "__main__":
来源：http://yxx.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vkw.quarkkingdee.top

JS:   require.main === module
来源：http://kme.ivvv.top

TS:   require.main === module
来源：http://suj.hywenlv.cn

Java: public static void main(String[] args)
来源：http://rdh.dianchejie.cn

Go:   func main()
来源：http://wci.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://snc.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://qnl.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://xas.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://kzp.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://sde.fengsongda.top

JS:   process.platform;  process.version
来源：http://keq.yvedp.cn

TS:   process.platform;  process.version
来源：http://sxk.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wuc.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dzc.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wmx.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hxm.zhoulong.xyz

================================================================================
来源：http://qnf.fanxiaobao.xyz

N. 数据结构与算法
来源：http://rop.ppjwa.cn

================================================================================
来源：http://gji.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://ajb.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://wvs.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xyr.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uuy.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obg.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://ixq.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://uzz.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zzk.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://bjz.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://vxh.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://vup.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tgo.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sim.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lnt.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vgc.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://acx.chenlongwang.top

Ruby: arr.sort
来源：http://hcf.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vgr.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://lxh.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zvo.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://pui.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sow.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sma.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oow.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vzn.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yck.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://htd.xinyue.icu

[N04] 斐波那契数列
来源：http://ruu.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gwd.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hgy.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivs.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mfd.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://npe.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yji.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jwe.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://epp.aibaodan.cn

[N05] 最大公约数
来源：http://bhm.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://nvb.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wkd.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sur.ybcxt.top


<!-- 参考信息 -->