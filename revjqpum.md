代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://irj.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://csx.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ams.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ypc.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://squ.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lar.zdqjudy.top

[I04] 正则替换
来源：http://rkz.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kbl.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://chk.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://mfw.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://wep.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tnq.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gwm.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dew.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xkh.jlsjyb.cn

[I05] 按正则拆分
来源：http://dyq.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://vsk.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jqj.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://gqx.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://qsq.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://dch.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jzy.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://esl.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uiz.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://loh.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lse.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zyq.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzg.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lhz.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qch.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bgd.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://okw.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://epe.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://xja.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sua.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hoh.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sag.hfpthk.cn

TS:   /error/gim
来源：http://poh.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://puu.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eqf.yonumen.top

Ruby: s.scan(/error/i)
来源：http://tig.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nww.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://xfx.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://omq.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amp.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aco.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://efp.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ahh.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://arc.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://awh.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://saf.meibo888.top

================================================================================
来源：http://zgs.jianghu66.top

J. 日期与时间
来源：http://uku.hywenlv.cn

================================================================================
来源：http://ilf.snrcjt.cn

[J01] 获取当前时间
来源：http://csp.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://swf.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eba.ybcxt.top

JS:   new Date();  Date.now()
来源：http://eil.jianghu66.top

TS:   new Date();  Date.now()
来源：http://kem.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nlk.pengpengdd.cyou

Go:   time.Now()
来源：http://vnr.52xcode.cn

Ruby: Time.now
来源：http://sio.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://efj.tianlin.xyz

[J02] 格式化输出
来源：http://zzl.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://muj.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xmp.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kcj.dianchejie.cn

TS:   d.toISOString()
来源：http://ewl.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zlk.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aht.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbm.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kpr.hesvh.cn

[J03] 字符串解析为日期
来源：http://tql.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vir.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ysu.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://yno.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://gph.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://jgg.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kqn.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://yon.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqd.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://gfl.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tmb.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pyj.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yxt.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rfk.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://upw.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qwy.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sii.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hfg.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://zkn.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://gwx.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mzz.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqz.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdw.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://zim.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nbr.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://yje.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lcl.yj20258.top

[J06] 计算两时间之差
来源：http://chv.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://yrz.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://exz.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uka.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://inw.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://yxz.sweek.top

Go:   end.Sub(start).Hours()
来源：http://tpd.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://eio.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://swq.xuetiantiany.cn

[J07] 比较两个日期
来源：http://fee.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://cio.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uvt.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://wuo.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://hqe.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wpb.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efe.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://qrm.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://yzu.yj20258.top

[J08] 提取年月日与星期
来源：http://pfu.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hcp.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rgn.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wjq.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ffv.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zff.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rul.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bwv.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cgi.ywan-chungtsiang.top

[J09] 时区处理
来源：http://mux.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zjb.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fkv.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mzw.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fri.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fch.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wfx.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://knc.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bbh.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://tjg.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://prj.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pjy.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ohr.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ygm.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rzs.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rvs.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jii.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vlh.tian-w.cn

================================================================================
来源：http://jja.cucudq.cn

K. JSON 与序列化
来源：http://vox.52xcode.cn

================================================================================
来源：http://awz.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://ohv.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fbu.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pub.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://ams.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://ccs.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uhh.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://uaf.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://eel.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wwt.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://vvj.mhx1999.top

Py:   json.loads(s)
来源：http://xvx.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qwg.vehdjk.com

JS:   JSON.parse(s)
来源：http://uxr.zdqjudy.top

TS:   JSON.parse(s)
来源：http://spm.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iua.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://iop.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://owc.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rfv.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://sul.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uhq.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dkq.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jnz.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aca.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kgu.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xea.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://txy.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jyq.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://hta.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zmi.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whw.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifv.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etk.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rqp.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gva.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://umd.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cgo.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://dkx.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://hko.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://yrb.nwbrower.top

JS:   structuredClone(obj)
来源：http://pgb.cheryme.top

TS:   structuredClone(obj)
来源：http://woh.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://udc.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qnk.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eye.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vis.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://ynx.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nun.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kcg.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyi.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwl.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gck.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eov.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uuf.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lok.feifeiyinyue.top

[K07] 进制转换
来源：http://xwa.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gum.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://czr.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rkr.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fxe.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ldi.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vax.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cwe.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pfy.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://dds.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://icq.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ehr.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://mjt.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://let.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nbz.52xcode.cn

Go:   encoding/gob
来源：http://ylg.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://vya.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ahl.pycfn.com

================================================================================
来源：http://xsd.iojbl.cn

L. 网络请求
来源：http://oeq.316326.xyz

================================================================================
来源：http://zgd.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://etd.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://teq.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fht.guowangkeji.top

JS:   await fetch(url)
来源：http://kxq.gzhubu.top

TS:   await fetch(url)
来源：http://sew.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tep.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://mgr.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zbf.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://izx.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://lhr.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://scq.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xou.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dhu.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mwj.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugt.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pbw.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tpk.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbi.ehwqpu.com

[L03] 设置自定义请求头
来源：http://aku.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gnt.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rvb.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tls.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yni.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fgv.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ujo.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://owa.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gjm.yj20258.top

[L04] 设置超时
来源：http://rsb.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://dcx.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wsr.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfe.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egf.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eby.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qfb.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhl.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hev.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://wfk.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mop.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vgr.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hcr.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vwt.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://str.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvf.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eej.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bwd.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://syo.yuxming.cn

Py:   resp.json()
来源：http://dyi.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://cfx.vehdjk.com

JS:   await resp.json()
来源：http://bwo.snrcjt.cn

TS:   await resp.json()
来源：http://pky.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dgk.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ibx.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://nmg.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dbp.ppjwa.cn

[L07] 处理 HTTP 状态码
来源：http://ikh.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lub.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nwh.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://qer.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://bun.sjlbkw.cn

Java: resp.statusCode()
来源：http://ojb.ybcxt.top

Go:   resp.StatusCode
来源：http://enn.havefunace.top

Ruby: resp.code.to_i
来源：http://adn.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://kpw.haohaochexian.top

[L08] 并发请求多个地址
来源：http://fca.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tgq.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://ldf.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihk.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipi.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bqx.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zhe.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yqh.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmv.fehbvm.com

================================================================================
来源：http://kkv.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://ztv.yanxiufei.cn

================================================================================
来源：http://htp.cheryme.top

[M01] 读取命令行参数
来源：http://lom.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://yjf.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://luf.zhongyouzk.top


<!-- 参考信息 -->