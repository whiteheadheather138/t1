代发 wailian999

================================================================================
来源：http://kqq.dianchejie.cn

I. 正则表达式
来源：http://aqy.iojbl.cn

================================================================================
来源：http://yyl.gzhubu.top

[I01] 判断是否匹配
来源：http://eia.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqa.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://ygn.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://cma.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://nih.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kcu.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://ppk.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xae.yj202588.top

[I02] 提取所有匹配
来源：http://iua.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://exq.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nxo.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jsb.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://ejb.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rwi.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iml.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://nst.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bin.yanxiufei.cn

[I03] 提取捕获分组
来源：http://fqa.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nxn.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fbn.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iuu.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eov.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vzp.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bhe.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lzv.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pse.hcnkem.com

[I04] 正则替换
来源：http://urs.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gyx.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kgn.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://vbm.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://goz.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://awb.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ohh.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vcn.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gfv.zhiwuduotai.top

[I05] 按正则拆分
来源：http://mft.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iag.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://weh.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://bkp.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://dgt.jlsjyb.cn

Java: s.split("\\s*,\\s*")
来源：http://kqf.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://clz.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://kwt.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgg.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qhu.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://niv.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cjr.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aij.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://daf.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wmc.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fhi.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zri.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wkz.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://wwy.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://obp.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gej.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uzr.jinqigufen.top

TS:   /error/gim
来源：http://klk.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dqe.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kzx.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://dzy.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhj.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://syb.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vzm.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wtp.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lwa.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ziv.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jbi.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jlg.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xyq.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://akj.shanyushiyangtech.top

================================================================================
来源：http://dql.chenzaomai.com

J. 日期与时间
来源：http://sxk.nanxinkj.top

================================================================================
来源：http://fbt.yongpay.top

[J01] 获取当前时间
来源：http://zwi.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jvs.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zub.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://niy.ydzc1.top

TS:   new Date();  Date.now()
来源：http://lyg.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://iom.chenzaomai.com

Go:   time.Now()
来源：http://wac.hcnkem.com

Ruby: Time.now
来源：http://iqa.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zmr.xuetiantiany.cn

[J02] 格式化输出
来源：http://jvq.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qdn.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gok.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xvc.sweek.top

TS:   d.toISOString()
来源：http://kae.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zeg.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nry.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lnt.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xxh.sufxvd.cn

[J03] 字符串解析为日期
来源：http://rjq.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fuf.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xgq.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://pkh.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://rzu.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://oxe.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gks.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://gzh.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yso.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://pbj.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqf.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ing.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kov.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hls.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://feo.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ciu.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pix.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cbt.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://wlp.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://qhq.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pga.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybz.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zta.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://oiv.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbe.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://sya.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://fbb.chenzaomai.com

[J06] 计算两时间之差
来源：http://kpk.cheryme.top

Py:   (end - start).total_seconds()
来源：http://ooj.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://rdp.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kpl.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyi.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://ttm.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://klu.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://nzi.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://xqw.xuetiantiany.cn

[J07] 比较两个日期
来源：http://wph.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://vra.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fxh.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xtr.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://hms.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iwe.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lch.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://vvd.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://dfa.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://byg.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uai.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jlz.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lee.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kbo.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yaf.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gzk.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vnf.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yht.tarul.cn

[J09] 时区处理
来源：http://abe.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://chm.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wmi.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://igm.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aix.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rlm.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iht.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://aci.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wfx.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://mck.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://adj.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://phy.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qwr.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kby.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nib.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://doi.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vgw.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qzb.pycfn.com

================================================================================
来源：http://tjq.gzhubu.top

K. JSON 与序列化
来源：http://xkp.zhengqikj.top

================================================================================
来源：http://oxy.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://nvf.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mno.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://txc.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://wiu.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://zly.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sig.sxryk.cn

Go:   json.Marshal(obj)
来源：http://gws.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://dnm.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uop.andypj.xyz

[K02] JSON 字符串转对象
来源：http://kns.yj20258.top

Py:   json.loads(s)
来源：http://fge.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fit.jiagoushi.top

JS:   JSON.parse(s)
来源：http://sav.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://obo.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ytv.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://lcj.daxiang520.top

Ruby: JSON.parse(s)
来源：http://gwc.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://knl.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://yoc.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wjr.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xqn.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://xyj.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://esw.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ykw.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fye.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://tqa.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://juw.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://tdb.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nbg.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qrc.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpx.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dgh.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kkc.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kmc.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rxi.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dih.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://loe.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://pnb.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://azc.andypj.xyz

JS:   structuredClone(obj)
来源：http://max.wangdashe.top

TS:   structuredClone(obj)
来源：http://mjd.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nph.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xll.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wik.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nhx.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://wqr.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ppt.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rvk.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xkf.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjk.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://juc.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rbl.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vzb.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vbj.jyoumei.cn

[K07] 进制转换
来源：http://fag.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wry.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ovb.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qeq.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cjp.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rlp.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tae.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lfe.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hcs.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://ors.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://apc.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gce.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://qnm.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://qgy.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://edz.yj20258888.top

Go:   encoding/gob
来源：http://eaw.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://kgg.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qng.zhoulong.xyz

================================================================================
来源：http://zgx.chenzaomai.com

L. 网络请求
来源：http://cel.uphjek.com

================================================================================
来源：http://nvd.andypj.xyz

[L01] 发送 GET 请求
来源：http://avo.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yqa.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jec.chenjidiqi.icu

JS:   await fetch(url)
来源：http://ala.jlsjyb.cn

TS:   await fetch(url)
来源：http://yyf.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lcf.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://ylz.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vzf.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jki.zdqjudy.top

[L02] 发送 POST JSON
来源：http://lrk.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://mdy.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jyr.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upy.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eiu.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://syk.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jxx.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vfq.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cpm.fengsongda.top

[L03] 设置自定义请求头
来源：http://vqg.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgr.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://knb.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lor.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xol.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pwk.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ste.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nhr.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gjh.pengpengdd.cyou

[L04] 设置超时
来源：http://lih.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://okr.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://twb.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wog.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xya.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sea.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qzw.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tce.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://itv.fktsv.cn

[L05] 上传文件（multipart）
来源：http://com.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dws.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dwn.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bok.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xpj.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mmj.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://odq.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://osn.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://liz.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://cta.xuetiantiany.cn

Py:   resp.json()
来源：http://bqe.yuxming.cn

PHP:  json_decode($body, true);
来源：http://cgm.jianghu66.top

JS:   await resp.json()
来源：http://jew.snrcjt.cn

TS:   await resp.json()
来源：http://com.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ymr.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vye.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://fch.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yma.zhoulong.xyz


<!-- 参考信息 -->