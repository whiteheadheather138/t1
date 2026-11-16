代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://puw.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://sqv.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://klv.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eut.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xzr.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gun.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bxo.iojbl.cn

[I05] 按正则拆分
来源：http://bur.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wvw.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gep.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://njj.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://lxc.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://xvb.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ibx.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://whp.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aut.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gbk.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oru.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gyl.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drs.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xil.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ozp.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lvg.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oic.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uob.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://fwj.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ydj.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ffv.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kus.dianchejie.cn

TS:   /error/gim
来源：http://dgs.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zfk.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rsh.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://fjh.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfg.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://jfo.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jqb.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fvp.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://edw.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://agh.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nsz.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xcq.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bhr.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wlt.redwolf501.top

================================================================================
来源：http://rqp.jlsjyb.cn

J. 日期与时间
来源：http://ooq.bjfxy.top

================================================================================
来源：http://rqp.yuxming.cn

[J01] 获取当前时间
来源：http://igc.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uvm.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qrf.tian-w.cn

JS:   new Date();  Date.now()
来源：http://kjp.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://wwl.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ehl.ydzc1.top

Go:   time.Now()
来源：http://qqh.gotoacloud.top

Ruby: Time.now
来源：http://kwo.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tjo.ybcxt.top

[J02] 格式化输出
来源：http://ruo.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iop.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vyp.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rpv.guannengcc.top

TS:   d.toISOString()
来源：http://tiy.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nxw.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hyc.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gcr.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qid.shzxlz.cn

[J03] 字符串解析为日期
来源：http://jns.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ufy.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pnn.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://aou.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://isa.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://mjr.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://twg.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://qrj.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kiy.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://ppr.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ign.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ojp.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hif.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://jbe.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gvv.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://onh.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kdg.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qbd.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://gxv.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://snv.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://whs.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mqw.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgb.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://pdo.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vaa.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://uzy.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ulf.sweek.top

[J06] 计算两时间之差
来源：http://irc.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://tsl.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://byv.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tos.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pgo.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://noa.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://cza.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://kwf.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://aqp.hammf.cn

[J07] 比较两个日期
来源：http://hku.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://mzw.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lkm.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://pcu.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://deb.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dnw.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qoj.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://yka.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://qdd.cucudq.cn

[J08] 提取年月日与星期
来源：http://upi.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bkx.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hcz.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://upu.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pix.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nvn.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tjg.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kun.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hlf.0kj1m.cn

[J09] 时区处理
来源：http://dyy.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ytx.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sof.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnw.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://skr.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ujf.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uye.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xbf.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bxw.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://bpo.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ubs.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jfj.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lud.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mcn.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yuj.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wob.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfa.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://axs.feifeiyinyue.top

================================================================================
来源：http://daa.hywenlv.cn

K. JSON 与序列化
来源：http://crp.shanyushiyangkeji.top

================================================================================
来源：http://zpb.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://yka.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wcl.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://scf.meibo888.top

JS:   JSON.stringify(obj)
来源：http://xub.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://xgm.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zvl.xinyue.icu

Go:   json.Marshal(obj)
来源：http://gzc.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://urk.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://olr.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://ekk.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://dqj.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nrq.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://afb.zhixingplan.top

TS:   JSON.parse(s)
来源：http://owt.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fuu.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://lun.yfazqb.com

Ruby: JSON.parse(s)
来源：http://nie.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ufa.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://miy.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ddn.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vuu.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://egg.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://exn.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sdf.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xnr.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://upl.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://azp.birdmap.top

[K04] 读取 JSON 文件
来源：http://hgn.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://usj.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ble.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdm.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://top.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nwv.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qio.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dth.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eja.pycfn.com

[K05] 深拷贝对象
来源：http://jwg.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://roo.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://six.xinyue.icu

JS:   structuredClone(obj)
来源：http://lqk.yj20258888.top

TS:   structuredClone(obj)
来源：http://syc.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fou.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://myx.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tre.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://sdb.cashguo.top

[K06] 解析 URL 查询串
来源：http://ook.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hcz.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ccm.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pku.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://swr.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://exh.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qdo.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xlo.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lef.kuanghao11.cn

[K07] 进制转换
来源：http://gur.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://afe.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://orx.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xzz.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://toy.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ksj.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://snt.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hxi.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ixr.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://lcj.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://tvm.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mjr.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://exj.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://uhx.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eyu.yuxming.cn

Go:   encoding/gob
来源：http://jfp.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://xsj.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfo.quarkkingdee.top

================================================================================
来源：http://ibo.vqdsnc.cn

L. 网络请求
来源：http://dxo.iojbl.cn

================================================================================
来源：http://twm.fktsv.cn

[L01] 发送 GET 请求
来源：http://zwz.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yvk.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mob.xziqi.cn

JS:   await fetch(url)
来源：http://mjs.tian-w.cn

TS:   await fetch(url)
来源：http://txz.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aar.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://qbv.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fga.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://opf.yj20258.top

[L02] 发送 POST JSON
来源：http://gcj.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uzn.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lwk.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tqe.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxb.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zli.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ilj.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yrz.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jmh.yuanzhike.top

[L03] 设置自定义请求头
来源：http://cyy.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ujr.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qfs.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rle.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rhj.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vmz.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wde.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qor.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rji.cqqwz.cn

[L04] 设置超时
来源：http://mki.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://crz.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qzw.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybj.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhz.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ntf.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wst.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wrw.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dio.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://wwm.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgp.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mhm.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwh.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lbz.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjr.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lms.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dwi.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cxf.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://xnu.shuidangran.top

Py:   resp.json()
来源：http://nou.redwolf501.top

PHP:  json_decode($body, true);
来源：http://bvr.epnwcf.com

JS:   await resp.json()
来源：http://lit.cdnleiting.top

TS:   await resp.json()
来源：http://fnp.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xuq.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bkz.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://zdi.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yoy.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://lpi.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ddr.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bal.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://akw.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://hnq.ctjpmb.com

Java: resp.statusCode()
来源：http://cls.nwbrower.top

Go:   resp.StatusCode
来源：http://jtm.yj202588.top

Ruby: resp.code.to_i
来源：http://ife.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://dww.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://sub.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sqv.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://xqd.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftt.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qor.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbm.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tvj.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pdh.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://olz.yj202588.top

================================================================================
来源：http://eih.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://ijv.yueranfly.top

================================================================================
来源：http://wrn.yj202588.top

[M01] 读取命令行参数
来源：http://tqw.tanke756.top

Py:   sys.argv[1:]
来源：http://eoy.bbcook.cn

PHP:  $argv;  $argc;
来源：http://ucc.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://pzu.hesvh.cn

TS:   process.argv.slice(2)
来源：http://zal.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://usq.daxiang520.top

Go:   os.Args[1:]
来源：http://axk.gzhubu.top

Ruby: ARGV
来源：http://lcc.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://hyd.9152youxi.cn

[M02] 读取环境变量
来源：http://ihd.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://tul.dianchejie.cn


<!-- 参考信息 -->