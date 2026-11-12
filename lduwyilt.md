代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://auy.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xfg.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ezw.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ebe.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://whz.xylfe.cn

[J08] 提取年月日与星期
来源：http://ddq.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ovw.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wsn.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wxq.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ipg.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://spx.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybx.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yxq.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://czb.zhiwuduotai.top

[J09] 时区处理
来源：http://yww.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dvn.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://adm.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ilv.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://etv.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nph.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://utm.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wva.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nfv.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://pay.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cjc.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwk.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vpi.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xnc.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qhn.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://crd.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gin.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pym.hysaishi.cn

================================================================================
来源：http://rkw.gzhubu.top

K. JSON 与序列化
来源：http://rzh.kuanghao11.cn

================================================================================
来源：http://hvi.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://wjn.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eaf.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xev.ivvv.top

JS:   JSON.stringify(obj)
来源：http://boj.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://vky.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xeu.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://lgo.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://sli.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://myq.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://zys.yonumen.top

Py:   json.loads(s)
来源：http://fuf.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tmr.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://bcl.birdmap.top

TS:   JSON.parse(s)
来源：http://mva.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sgz.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fby.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://zec.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iqf.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://lxq.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://isr.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wwy.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ogw.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vup.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mma.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rkc.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://pgu.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eqz.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://xqw.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rav.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aqf.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvq.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qro.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xfg.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qde.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nwz.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xjp.hnxiangtu.top

[K05] 深拷贝对象
来源：http://nst.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://mux.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://zxi.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://xex.fehbvm.com

TS:   structuredClone(obj)
来源：http://lku.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jgr.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tqp.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgg.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zsk.c1oappe.top

[K06] 解析 URL 查询串
来源：http://oiw.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kju.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yby.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://msy.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vjp.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://djp.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wsx.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dyh.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pou.hnqzz.top

[K07] 进制转换
来源：http://rbx.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fuj.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pxf.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ing.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hvx.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tet.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ppw.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://juj.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ruz.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://uhb.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://xcb.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ont.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://qhi.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://nfh.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://znd.ydzc1.top

Go:   encoding/gob
来源：http://jvu.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://ipd.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oqm.yongpay.top

================================================================================
来源：http://eew.jianghu66.top

L. 网络请求
来源：http://ljs.redwolf501.top

================================================================================
来源：http://zlh.shuidangran.top

[L01] 发送 GET 请求
来源：http://lqy.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pdu.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://est.9152youxi.cn

JS:   await fetch(url)
来源：http://quy.quarkkingdee.top

TS:   await fetch(url)
来源：http://dxu.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lai.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://dvu.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lpq.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qqe.0kj1m.cn

[L02] 发送 POST JSON
来源：http://gam.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zrh.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://odo.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wuv.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uku.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://frf.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aay.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bft.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vyd.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://wcl.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xwb.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xiq.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://szf.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyy.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hjr.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://emg.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eov.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pzq.sxryk.cn

[L04] 设置超时
来源：http://lka.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://fbv.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fal.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ptb.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sao.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xiv.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bum.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mrc.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://erp.fktsv.cn

[L05] 上传文件（multipart）
来源：http://lst.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://khp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oam.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ynw.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kwm.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uxd.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aes.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://abh.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tug.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://ixr.cheryme.top

Py:   resp.json()
来源：http://his.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://ndd.fehbvm.com

JS:   await resp.json()
来源：http://obb.yuanzhike.top

TS:   await resp.json()
来源：http://xfh.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vnj.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qhl.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://mpi.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sla.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://zdu.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zle.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rpe.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://yxh.meibo888.top

TS:   resp.ok;  resp.status
来源：http://uom.jianghu66.top

Java: resp.statusCode()
来源：http://icj.gogol.net.cn

Go:   resp.StatusCode
来源：http://erm.tianlin.xyz

Ruby: resp.code.to_i
来源：http://dbo.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://uje.ppjwa.cn

[L08] 并发请求多个地址
来源：http://xjr.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uiv.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://kci.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwz.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkh.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xln.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xic.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avn.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kcl.yangfankeji.com

================================================================================
来源：http://jkg.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://zpg.feifeiyinyue.top

================================================================================
来源：http://whe.epnwcf.com

[M01] 读取命令行参数
来源：http://huc.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://hum.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://jvn.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://msw.daria6918.cn

TS:   process.argv.slice(2)
来源：http://yjv.uphjek.com

Java: args 数组（main 方法参数）
来源：http://yuo.pycfn.com

Go:   os.Args[1:]
来源：http://spo.redwolf501.top

Ruby: ARGV
来源：http://jmu.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://yhk.shangyingyoupin.top

[M02] 读取环境变量
来源：http://rgo.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://pzn.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lzu.quarkkingdee.top

JS:   process.env.HOME
来源：http://anj.smart0.xyz

TS:   process.env.HOME
来源：http://mvn.0kj1m.cn

Java: System.getenv("HOME")
来源：http://bdd.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cmx.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://ndz.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zgd.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://jlz.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oln.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxs.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ror.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xtg.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hak.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kdg.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://woq.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://jbc.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://mlv.ivvv.top

Py:   os.getcwd()
来源：http://bko.cqqwz.cn

PHP:  getcwd();
来源：http://tpi.tanke756.top

JS:   process.cwd()
来源：http://dza.tian-w.cn

TS:   process.cwd()
来源：http://oai.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://ikf.hywenlv.cn

Go:   os.Getwd()
来源：http://rnj.zhongyouzk.top

Ruby: Dir.pwd
来源：http://zdo.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xgz.hfpthk.cn

[M05] 设置退出码
来源：http://uas.xylfe.cn

Py:   sys.exit(1)
来源：http://lkf.pycfn.com

PHP:  exit(1);
来源：http://jqs.yonumen.top

JS:   process.exit(1)
来源：http://xbr.zhongyouzk.top

TS:   process.exit(1)
来源：http://cwm.tianlin.xyz

Java: System.exit(1)
来源：http://kyi.nanxinkj.top

Go:   os.Exit(1)
来源：http://que.chenlongwang.top

Ruby: exit 1
来源：http://uia.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://trd.gotoacloud.top

[M06] 向标准错误输出
来源：http://byi.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://chc.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://irj.gogol.net.cn

JS:   console.error("err")
来源：http://gwz.cdnleiting.top

TS:   console.error("err")
来源：http://qte.tian-w.cn

Java: System.err.println("err")
来源：http://xsj.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dpm.fehbvm.com

Ruby: warn "err"
来源：http://epr.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://jva.yonumen.top

[M07] 判断是否为主入口
来源：http://ijl.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://afh.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gbp.tarul.cn

JS:   require.main === module
来源：http://nxr.ivvv.top

TS:   require.main === module
来源：http://bwf.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://btr.9152youxi.cn

Go:   func main()
来源：http://pcd.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbt.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://evj.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://mme.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://kev.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://zfm.sysykeji.top

JS:   process.platform;  process.version
来源：http://nfy.birdmap.top

TS:   process.platform;  process.version
来源：http://ptp.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dmc.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nho.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gwm.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zrp.yj202588.top

================================================================================
来源：http://nrp.yanxiufei.cn

N. 数据结构与算法
来源：http://oel.zhongyouzk.top

================================================================================
来源：http://tcp.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://xye.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://erb.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nri.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obo.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vkf.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://emm.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://xim.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xxs.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://jwt.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://vqk.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://kvl.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://odl.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://puz.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ftq.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://guu.bbcook.cn

Go:   slices.Sort(arr)
来源：http://yar.yfazqb.com

Ruby: arr.sort
来源：http://bao.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://boy.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://gtb.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sux.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://mkz.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pfs.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lsg.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ogc.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ybi.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lpu.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://cdg.yj202588.top

[N04] 斐波那契数列
来源：http://xex.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lal.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lhc.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lxg.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gjo.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fwb.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aur.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uph.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mxw.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://mnl.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://itk.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gdn.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nrv.zhongyouzk.top


<!-- 参考信息 -->