代发 wailian999

[I02] 提取所有匹配
来源：http://pmb.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://joh.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zwm.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bnn.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://rid.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://alm.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mri.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://cpx.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ehy.uphjek.com

[I03] 提取捕获分组
来源：http://xxs.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jdz.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qha.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jlz.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://llm.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdl.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vey.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fzi.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kfr.316326.xyz

[I04] 正则替换
来源：http://hpu.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qcf.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmj.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wkj.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://tme.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://dee.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bss.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ugv.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bwp.zhiwuduotai.top

[I05] 按正则拆分
来源：http://ggj.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xfo.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gjp.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://gjz.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://pml.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://vxi.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brf.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uyw.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pqv.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://doq.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oft.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oec.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kgq.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iph.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://smg.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://llw.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hyg.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://plp.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://qer.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hlg.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twb.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wrf.pengpengdd.cyou

TS:   /error/gim
来源：http://srn.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pea.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xzs.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://wpr.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zxy.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://ccb.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lif.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nzi.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ico.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mol.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jcw.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://des.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwr.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tui.jinyuanbaomall.cn

================================================================================
来源：http://qsd.yj202588.top

J. 日期与时间
来源：http://rax.epnwcf.com

================================================================================
来源：http://kso.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://znl.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wtn.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cxm.bjfxy.top

JS:   new Date();  Date.now()
来源：http://uiv.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://nod.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jpb.yonumen.top

Go:   time.Now()
来源：http://wld.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://bfx.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yyj.c1oappe.top

[J02] 格式化输出
来源：http://vlh.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://acr.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iis.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://avd.shangyingyoupin.top

TS:   d.toISOString()
来源：http://yxy.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nhm.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kll.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nbu.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvi.gotoacloud.top

[J03] 字符串解析为日期
来源：http://nkf.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ydm.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kex.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://shg.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://rwu.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://icv.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdn.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://npw.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nnw.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://hto.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gix.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://abq.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://byd.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ksr.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uhg.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://raa.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cfr.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hif.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://hon.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://pui.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zgn.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsv.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryc.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ysc.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wsr.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://jyw.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://emp.sxryk.cn

[J06] 计算两时间之差
来源：http://vyf.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://med.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://nkk.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rxm.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nef.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bhx.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://syl.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://bga.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://huo.dianchejie.cn

[J07] 比较两个日期
来源：http://ine.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://lpq.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uxd.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://zgi.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://ywu.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ekf.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kev.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pie.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://vod.shzxlz.cn

[J08] 提取年月日与星期
来源：http://dmi.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rzf.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dnr.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mtt.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://edi.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tcc.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eyc.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://djh.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zxz.zhijiandao.cn

[J09] 时区处理
来源：http://xdx.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gyw.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rwb.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hep.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxh.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://omh.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://npp.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kad.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://haz.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://zjv.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gei.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fvj.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfh.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ryp.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fnx.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wvb.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iry.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwl.shzxlz.cn

================================================================================
来源：http://qhb.ivvv.top

K. JSON 与序列化
来源：http://dmk.daxiang520.top

================================================================================
来源：http://too.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://sim.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zmg.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zwe.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://hex.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://mcy.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wlo.ybcxt.top

Go:   json.Marshal(obj)
来源：http://zjb.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://srx.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eit.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://hsn.0kj1m.cn

Py:   json.loads(s)
来源：http://elu.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vzv.uphjek.com

JS:   JSON.parse(s)
来源：http://nck.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://vqp.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gni.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://xnh.sweek.top

Ruby: JSON.parse(s)
来源：http://bth.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dws.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://awg.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vyq.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rtp.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://wtc.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ato.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ypi.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wko.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ngy.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ipi.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://jzo.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xlq.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzs.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://boy.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zyh.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vqn.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbt.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tdw.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lka.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://rst.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://gid.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://nsj.smart0.xyz

JS:   structuredClone(obj)
来源：http://clc.uphjek.com

TS:   structuredClone(obj)
来源：http://yun.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://khl.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gli.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://flc.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kev.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://exw.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jhm.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://val.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tru.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qbf.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gwb.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://tkg.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oxy.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jaq.hywenlv.cn

[K07] 进制转换
来源：http://lpf.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ajk.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://moz.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dmr.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://glu.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ppk.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xvk.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ptm.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmo.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://rwm.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://vty.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vmp.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://wel.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://qqy.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hdm.jiagoushi.top

Go:   encoding/gob
来源：http://vnj.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://cds.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eyv.shzxlz.cn

================================================================================
来源：http://tlk.nanxuanxn.top

L. 网络请求
来源：http://mba.hywenlv.cn

================================================================================
来源：http://ean.cashguo.top

[L01] 发送 GET 请求
来源：http://oxw.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmf.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ajp.smart0.xyz

JS:   await fetch(url)
来源：http://uuo.tanke756.top

TS:   await fetch(url)
来源：http://wlw.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pfq.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://jgt.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bdg.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fax.yj20258.top

[L02] 发送 POST JSON
来源：http://kza.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://tif.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fyn.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xho.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foc.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfm.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zzw.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ugp.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tuw.fengsongda.top

[L03] 设置自定义请求头
来源：http://rrn.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://drn.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vir.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbu.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsp.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://atv.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sat.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfe.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tvy.hysaishi.cn

[L04] 设置超时
来源：http://kha.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://kkm.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yrr.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://alx.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwm.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tdw.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://whq.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mwt.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yez.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://aob.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://onb.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zcn.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tgz.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://itq.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eet.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nrw.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asc.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://syk.aizwys.cn

[L06] 解析响应为 JSON
来源：http://xzy.cucudq.cn

Py:   resp.json()
来源：http://zgi.nwbrower.top

PHP:  json_decode($body, true);
来源：http://zht.zhiwuduotai.top

JS:   await resp.json()
来源：http://pjo.yonumen.top

TS:   await resp.json()
来源：http://uay.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dns.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jja.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://thk.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixj.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://qxh.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kwy.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://krl.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://fki.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://onv.daria6918.cn

Java: resp.statusCode()
来源：http://zub.birdmap.top

Go:   resp.StatusCode
来源：http://zfi.sysykeji.top

Ruby: resp.code.to_i
来源：http://gcr.cashguo.top

C#:   (int)resp.StatusCode
来源：http://xai.fengsongda.top

[L08] 并发请求多个地址
来源：http://npg.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jeh.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://qgt.wangdashe.top


<!-- 参考信息 -->