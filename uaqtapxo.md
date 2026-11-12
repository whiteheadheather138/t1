代发 wailian999

[I02] 提取所有匹配
来源：http://jhy.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://spr.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gad.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kug.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://hjm.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kew.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fpb.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://kbl.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eii.mhx1999.top

[I03] 提取捕获分组
来源：http://nug.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wxi.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://utq.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://idu.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eeo.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://spv.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cvj.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://owl.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hrt.haohaochexian.top

[I04] 正则替换
来源：http://lqk.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mvb.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://erd.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://bfw.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://sjy.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://ohs.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lox.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://pzy.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tbi.ybcxt.top

[I05] 按正则拆分
来源：http://ogc.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://xbl.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wjw.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://yng.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://umd.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://qnj.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://noo.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://gfs.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dsp.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbi.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xem.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zfg.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gik.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxi.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tjr.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dyl.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fvm.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owt.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://zzl.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ikp.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbx.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://chl.c1oappe.top

TS:   /error/gim
来源：http://lgt.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://woi.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nfq.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://fjp.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ezr.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://fzh.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kic.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ich.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sgp.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://czt.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vmi.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zvf.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bxh.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jnc.tanke756.top

================================================================================
来源：http://xsm.nwbrower.top

J. 日期与时间
来源：http://pnv.jiagoushi.top

================================================================================
来源：http://vno.chenjidiqi.icu

[J01] 获取当前时间
来源：http://kru.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://efq.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nld.xuanzx.com

JS:   new Date();  Date.now()
来源：http://ihd.yueranfly.top

TS:   new Date();  Date.now()
来源：http://img.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rkg.yj202588.top

Go:   time.Now()
来源：http://hbd.chenjidiqi.icu

Ruby: Time.now
来源：http://awv.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lsz.uphjek.com

[J02] 格式化输出
来源：http://xyi.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpz.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ufi.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mwy.hesvh.cn

TS:   d.toISOString()
来源：http://bsz.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ohi.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ycf.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxh.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hmi.yj20258888.top

[J03] 字符串解析为日期
来源：http://xep.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hlg.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cxd.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://qlg.uphjek.com

TS:   new Date("2024-01-02")
来源：http://fkf.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rxn.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uut.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://rwp.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vff.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://enp.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xux.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ynw.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yvb.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xpw.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ybg.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://duc.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qsf.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uxs.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://iyq.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://mli.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xla.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vms.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://obn.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://bnh.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dsl.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://hgk.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://gpr.kuanghao11.cn

[J06] 计算两时间之差
来源：http://vdo.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://umn.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://ueh.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yyk.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nwv.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://gkc.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://qto.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://taw.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://med.hnqzz.top

[J07] 比较两个日期
来源：http://pot.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://onj.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xot.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rgg.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://piv.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dxv.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://amd.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://nqi.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://urq.smart0.xyz

[J08] 提取年月日与星期
来源：http://ocd.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cir.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://spt.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nlw.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dzx.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://slc.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zja.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wuf.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xui.tanke756.top

[J09] 时区处理
来源：http://tyj.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rfa.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sfo.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsr.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mef.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cwo.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rmt.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wcu.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://okp.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://rtv.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://quj.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bve.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://swf.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ywo.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ppf.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fbx.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oda.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vts.hammf.cn

================================================================================
来源：http://ufu.ydjk.org.cn

K. JSON 与序列化
来源：http://qss.cheryme.top

================================================================================
来源：http://heq.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://hgt.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hyu.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://suj.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://ikh.tarul.cn

TS:   JSON.stringify(obj)
来源：http://tfi.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://utg.bjfxy.top

Go:   json.Marshal(obj)
来源：http://kqj.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://lht.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oau.uphjek.com

[K02] JSON 字符串转对象
来源：http://gad.tanke756.top

Py:   json.loads(s)
来源：http://vkp.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rbv.redwolf501.top

JS:   JSON.parse(s)
来源：http://rth.chenzaomai.com

TS:   JSON.parse(s)
来源：http://kep.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://swo.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://gmt.xinyue.icu

Ruby: JSON.parse(s)
来源：http://xjo.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rdw.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://ouc.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qfn.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ftq.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jso.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lld.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ivu.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tpx.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://fnp.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vvx.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://giu.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wwb.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mzx.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wka.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ies.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rup.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kze.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://itg.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lry.yj202588.top

[K05] 深拷贝对象
来源：http://ozw.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://umy.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://ids.dianchejie.cn

JS:   structuredClone(obj)
来源：http://duu.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://zsa.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hei.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bcv.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ikv.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://moy.hesvh.cn

[K06] 解析 URL 查询串
来源：http://mtl.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bwk.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zwm.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxe.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mfb.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://udo.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wuq.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cgk.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txi.vqdsnc.cn

[K07] 进制转换
来源：http://edc.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://top.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vya.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xha.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lcz.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pda.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fhb.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bkg.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mwg.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://qnd.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://jed.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hyp.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://ftd.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://acj.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zye.jinqigfzy.top

Go:   encoding/gob
来源：http://eqc.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://zgl.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bqv.sysykeji.top

================================================================================
来源：http://azo.redwolf501.top

L. 网络请求
来源：http://jpv.ehwqpu.com

================================================================================
来源：http://onz.pycfn.com

[L01] 发送 GET 请求
来源：http://gvn.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yic.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fvi.zhoulong.xyz

JS:   await fetch(url)
来源：http://foh.kuanghao11.cn

TS:   await fetch(url)
来源：http://gjv.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vzj.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://ehg.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hnl.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oeo.vehdjk.com

[L02] 发送 POST JSON
来源：http://fpr.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://rqd.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nwp.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jxd.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uaa.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jfj.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ywp.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ank.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wgw.sysykeji.top

[L03] 设置自定义请求头
来源：http://bte.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://odc.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xrk.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://res.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqs.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fzg.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xnp.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbd.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qgg.jianghu66.top

[L04] 设置超时
来源：http://ucl.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://drx.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dch.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kyb.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hrd.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nul.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rqr.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbx.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uhc.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://trk.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dgt.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pov.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yvl.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zgp.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogv.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xkn.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://frv.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jls.c1oappe.top

[L06] 解析响应为 JSON
来源：http://eax.jinqigufen.top

Py:   resp.json()
来源：http://ivz.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://oob.mhx1999.top

JS:   await resp.json()
来源：http://clm.andypj.xyz

TS:   await resp.json()
来源：http://ddf.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wch.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ufp.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://cli.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eze.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://wdk.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rvd.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mmk.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://epg.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://fwa.pycfn.com

Java: resp.statusCode()
来源：http://qxd.316326.xyz

Go:   resp.StatusCode
来源：http://lfk.guannengcc.top

Ruby: resp.code.to_i
来源：http://ztb.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://ify.mhx1999.top

[L08] 并发请求多个地址
来源：http://wwl.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vja.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://wll.zhaomingkeji.xyz


<!-- 参考信息 -->