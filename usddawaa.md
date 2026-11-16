代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gwj.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://fvl.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://eey.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://bxv.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uzb.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qnd.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://lri.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wsw.ehwqpu.com

[I02] 提取所有匹配
来源：http://fhe.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://jzr.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sji.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pvp.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://gcf.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://osl.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ugy.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://pno.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dcj.316326.xyz

[I03] 提取捕获分组
来源：http://ccp.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://feh.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xsa.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwr.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ysg.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kor.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xqr.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lfs.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vat.ppjwa.cn

[I04] 正则替换
来源：http://aqe.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://omt.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wga.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://eva.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://vtk.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zdn.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://blj.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://jhu.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://efh.sxryk.cn

[I05] 按正则拆分
来源：http://eau.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jmb.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rgd.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://qyd.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://ucb.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://cfw.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kpd.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ylt.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rcq.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nha.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://auw.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jla.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ogo.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzr.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://djf.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpe.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ble.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sbb.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://iyr.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yek.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hqp.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ewq.cqqwz.cn

TS:   /error/gim
来源：http://ceb.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mvl.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wox.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://zty.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bar.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://uci.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dmb.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://war.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbg.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://per.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dan.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sau.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kst.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ibt.fzhhl.top

================================================================================
来源：http://wiv.ydjk.org.cn

J. 日期与时间
来源：http://vfr.yuanzhike.top

================================================================================
来源：http://lme.tian-w.cn

[J01] 获取当前时间
来源：http://eae.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lcg.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ovw.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://liu.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://taa.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nhi.guannengcc.top

Go:   time.Now()
来源：http://iek.gzhubu.top

Ruby: Time.now
来源：http://gnw.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aho.yj20258.top

[J02] 格式化输出
来源：http://qgf.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://esr.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lun.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mgm.cashguo.top

TS:   d.toISOString()
来源：http://goi.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wnt.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://del.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cvp.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dyd.nanxinkj.top

[J03] 字符串解析为日期
来源：http://hbr.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ztp.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dyf.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://qwt.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://njh.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://mxc.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvm.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xmi.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yzm.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://fvq.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fgj.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jey.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gbb.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zcj.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wgo.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vlk.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ijt.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjk.sweek.top

[J05] 时间加减（加 7 天）
来源：http://wwg.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://hwp.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lza.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izg.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sft.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://rlo.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sqc.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://iil.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://glc.jyoumei.cn

[J06] 计算两时间之差
来源：http://zeh.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://qge.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://wbv.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qos.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kcn.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ahx.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://tdi.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://mnt.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://lul.cucudq.cn

[J07] 比较两个日期
来源：http://dje.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://fvr.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bzv.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://gar.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://jac.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ocw.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dop.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gom.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://xzr.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://pka.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tgf.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lki.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jly.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hlw.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kmn.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lhk.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://naw.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fzb.hfpthk.cn

[J09] 时区处理
来源：http://wus.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bnw.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yvp.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtn.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utn.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://leg.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jnu.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xiu.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ksg.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://esk.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mdh.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lou.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pws.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bbs.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://caa.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ddo.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://auw.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mfl.xuetiantiany.cn

================================================================================
来源：http://uud.iojbl.cn

K. JSON 与序列化
来源：http://ptk.wangshuangyany.cn

================================================================================
来源：http://euf.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://joz.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iie.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://umf.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://zde.tanke756.top

TS:   JSON.stringify(obj)
来源：http://qbd.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cin.daria6918.cn

Go:   json.Marshal(obj)
来源：http://rzn.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://cxc.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lod.uphjek.com

[K02] JSON 字符串转对象
来源：http://gpu.pengpengdd.cyou

Py:   json.loads(s)
来源：http://rsq.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oyt.dashuyun.cn

JS:   JSON.parse(s)
来源：http://vqs.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://hpu.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dru.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://aba.tian-w.cn

Ruby: JSON.parse(s)
来源：http://qyw.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iqe.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://gdr.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zix.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://frc.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lmc.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wrh.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://efx.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sgl.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kyy.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://npx.yj20258.top

[K04] 读取 JSON 文件
来源：http://jws.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wgt.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://srp.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://slp.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qso.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sfj.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iou.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uto.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://soa.mhx1999.top

[K05] 深拷贝对象
来源：http://ktp.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://jee.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://wtk.yuanzhike.top

JS:   structuredClone(obj)
来源：http://gak.zycfv.cn

TS:   structuredClone(obj)
来源：http://uje.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ifd.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jiq.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uvp.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uek.pycfn.com

[K06] 解析 URL 查询串
来源：http://qic.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zjs.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fex.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bxw.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zpq.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://clw.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aqo.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kgo.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jtb.cashguo.top

[K07] 进制转换
来源：http://xyy.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hil.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wvx.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://syl.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kmv.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rae.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mep.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uer.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://whe.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://yfv.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://qpp.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tjq.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://gba.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://jqx.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iyz.chenzaomai.com

Go:   encoding/gob
来源：http://bar.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://wmd.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vkr.cqqwz.cn

================================================================================
来源：http://wsf.vehdjk.com

L. 网络请求
来源：http://ufx.guannengcc.top

================================================================================
来源：http://hpx.tarul.cn

[L01] 发送 GET 请求
来源：http://tod.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gts.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://shp.cheryme.top

JS:   await fetch(url)
来源：http://glu.c1oappe.top

TS:   await fetch(url)
来源：http://tqj.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://otp.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://pyk.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://vnd.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ahe.jyoumei.cn

[L02] 发送 POST JSON
来源：http://rsg.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sav.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bzm.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dmu.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lmk.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kcz.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://epc.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vte.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fmg.sweek.top

[L03] 设置自定义请求头
来源：http://ybt.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kcc.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zic.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxz.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kop.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eil.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hst.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hhf.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://boz.zhoulong.xyz

[L04] 设置超时
来源：http://ygw.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://anm.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://slu.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dqn.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsb.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odb.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qbm.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kxt.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdu.tarul.cn

[L05] 上传文件（multipart）
来源：http://xtu.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tti.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zty.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxm.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rdz.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ujn.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xba.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nzb.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wgb.bbcook.cn

[L06] 解析响应为 JSON
来源：http://fyq.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://veu.shuidangran.top

PHP:  json_decode($body, true);
来源：http://qit.smart0.xyz

JS:   await resp.json()
来源：http://nvk.yanxiufei.cn

TS:   await resp.json()
来源：http://mzw.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouy.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fhu.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://aog.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yye.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://zgs.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lno.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dor.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://ydb.chenzaomai.com


<!-- 参考信息 -->