代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://jcl.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ifj.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ttb.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://kxe.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://dbg.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://enb.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://set.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ccs.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fos.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fgj.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rnn.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jcp.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wch.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wpc.quarkkingdee.top

[J09] 时区处理
来源：http://uvz.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://coi.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://abk.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfk.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbk.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lze.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jeg.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gri.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wvj.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://tnd.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eet.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sle.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dpl.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zaf.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oji.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qbp.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqv.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aev.aizwys.cn

================================================================================
来源：http://bvs.shanyushiyangtech.top

K. JSON 与序列化
来源：http://nke.jlsjyb.cn

================================================================================
来源：http://tcd.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://bzz.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dfm.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://liq.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://slx.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://eht.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wux.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://qzc.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://pat.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pto.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://mto.birdmap.top

Py:   json.loads(s)
来源：http://hwh.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://stw.uphjek.com

JS:   JSON.parse(s)
来源：http://giz.zycfv.cn

TS:   JSON.parse(s)
来源：http://vkj.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzr.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://ife.vehdjk.com

Ruby: JSON.parse(s)
来源：http://jds.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://osn.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://qjx.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hde.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exi.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wla.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bgo.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zxd.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xcm.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://sow.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://brw.wangdashe.top

[K04] 读取 JSON 文件
来源：http://gjg.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aef.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ybv.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gtx.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nft.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpt.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://izu.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ikj.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://exb.tianlin.xyz

[K05] 深拷贝对象
来源：http://set.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://iak.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://opp.epnwcf.com

JS:   structuredClone(obj)
来源：http://tzf.fzhhl.top

TS:   structuredClone(obj)
来源：http://sxy.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://awd.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ilv.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ycc.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://izx.hnqzz.top

[K06] 解析 URL 查询串
来源：http://osj.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ime.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dvg.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axf.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://itp.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qsu.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://knx.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cei.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xro.vehdjk.com

[K07] 进制转换
来源：http://yeq.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ood.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzm.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bct.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hic.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://seb.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://txl.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://etq.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zkf.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://uwe.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://njn.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ulu.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://xph.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://mwj.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgm.fktsv.cn

Go:   encoding/gob
来源：http://hcs.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://cvb.tian-w.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://klm.yuanzhike.top

================================================================================
来源：http://evo.yuxming.cn

L. 网络请求
来源：http://eyh.jiagoushi.top

================================================================================
来源：http://jug.gotoacloud.top

[L01] 发送 GET 请求
来源：http://mvd.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mwj.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hcf.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://icd.cqqwz.cn

TS:   await fetch(url)
来源：http://trm.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tvf.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://xea.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oaa.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mea.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://aae.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://szw.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://edh.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lpz.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tmv.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aqc.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ggh.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tpb.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kzm.chenlongwang.top

[L03] 设置自定义请求头
来源：http://bgq.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pms.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jmm.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpj.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bgk.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dol.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ydj.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xew.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tnr.ehwqpu.com

[L04] 设置超时
来源：http://czo.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://eqf.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pkj.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvv.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nms.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yab.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lxx.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dsc.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wkl.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://iob.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgg.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ixw.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uza.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mwt.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cdq.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yld.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://leb.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npm.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://ibr.ydzc1.top

Py:   resp.json()
来源：http://nxk.jianghu66.top

PHP:  json_decode($body, true);
来源：http://nln.chenzaomai.com

JS:   await resp.json()
来源：http://jkv.cucudq.cn

TS:   await resp.json()
来源：http://qrs.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zns.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cgj.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://inc.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ccu.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://eft.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tcj.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spd.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://pzr.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://klk.tianlin.xyz

Java: resp.statusCode()
来源：http://vvu.aibaodan.cn

Go:   resp.StatusCode
来源：http://ibk.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://iys.meibo888.top

C#:   (int)resp.StatusCode
来源：http://oos.gotoacloud.top

[L08] 并发请求多个地址
来源：http://hqf.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ytj.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://tsv.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uyn.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uyz.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qfi.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fxq.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://emr.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qsp.yonumen.top

================================================================================
来源：http://rnp.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://iol.zhijiandao.cn

================================================================================
来源：http://etw.ehwqpu.com

[M01] 读取命令行参数
来源：http://see.ybcxt.top

Py:   sys.argv[1:]
来源：http://ywx.tarul.cn

PHP:  $argv;  $argc;
来源：http://oau.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://ost.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://htq.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://ipb.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://wpz.jqgfzy.top

Ruby: ARGV
来源：http://tkm.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://myt.jyoumei.cn

[M02] 读取环境变量
来源：http://bqm.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://skb.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hqg.bbcook.cn

JS:   process.env.HOME
来源：http://ouv.ehwqpu.com

TS:   process.env.HOME
来源：http://adf.wangdashe.top

Java: System.getenv("HOME")
来源：http://zwc.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ilt.yvedp.cn

Ruby: ENV["HOME"]
来源：http://owu.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://irs.52xcode.cn

[M03] 执行外部命令
来源：http://hst.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aiv.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dpn.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bky.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dky.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://acz.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qik.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://zja.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://mnm.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://oml.uphjek.com

Py:   os.getcwd()
来源：http://eqz.9152youxi.cn

PHP:  getcwd();
来源：http://sbi.jinghuilouyu.cn

JS:   process.cwd()
来源：http://rjd.zhiwuduotai.top

TS:   process.cwd()
来源：http://hlk.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://csu.fktsv.cn

Go:   os.Getwd()
来源：http://ubv.pycfn.com

Ruby: Dir.pwd
来源：http://mmi.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://kum.kuanghao11.cn

[M05] 设置退出码
来源：http://nnf.zdqjudy.top

Py:   sys.exit(1)
来源：http://wpp.yfazqb.com

PHP:  exit(1);
来源：http://lgm.snrcjt.cn

JS:   process.exit(1)
来源：http://ydt.wangshuangyany.cn

TS:   process.exit(1)
来源：http://rzq.nwbrower.top

Java: System.exit(1)
来源：http://qmd.cheryme.top

Go:   os.Exit(1)
来源：http://opv.316326.xyz

Ruby: exit 1
来源：http://dsh.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://omk.pycfn.com

[M06] 向标准错误输出
来源：http://qeo.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://jpk.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://syj.zhengqikj.top

JS:   console.error("err")
来源：http://nqz.ctjpmb.com

TS:   console.error("err")
来源：http://xlh.cucudq.cn

Java: System.err.println("err")
来源：http://njx.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xej.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://gsk.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://nvq.birdmap.top

[M07] 判断是否为主入口
来源：http://kkd.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://qoa.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wvg.gzhubu.top

JS:   require.main === module
来源：http://kbd.sysykeji.top

TS:   require.main === module
来源：http://cdr.dashuyun.cn

Java: public static void main(String[] args)
来源：http://cat.jinqigufen.top

Go:   func main()
来源：http://jga.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://huf.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://exm.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://yrq.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://wmh.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://ocj.cqqwz.cn

JS:   process.platform;  process.version
来源：http://xof.snrcjt.cn

TS:   process.platform;  process.version
来源：http://uzu.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kdj.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zrx.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zyi.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://toi.snrcjt.cn

================================================================================
来源：http://sxw.sweek.top

N. 数据结构与算法
来源：http://qlk.yj20258.top

================================================================================
来源：http://eru.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://ufn.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jus.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tgx.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwy.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snf.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://dwf.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://kmq.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ztc.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kfa.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://iql.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://akx.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qnr.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cdg.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lwk.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://llh.yj20258888.top

Go:   slices.Sort(arr)
来源：http://hhj.pengpengdd.cyou

Ruby: arr.sort
来源：http://fwd.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://rsz.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://lus.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wag.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://kzf.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jfc.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbb.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ebf.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://avl.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyx.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://tjo.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://fvj.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxz.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yse.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gap.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tah.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zmg.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dlt.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yup.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rkp.zdbjq.cn

[N05] 最大公约数
来源：http://fan.hesvh.cn

Py:   math.gcd(a, b)
来源：http://tvq.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fdg.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wxd.yfazqb.com


<!-- 参考信息 -->