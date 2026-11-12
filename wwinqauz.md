代发 wailian999

================================================================================
来源：http://agq.havefunace.top

I. 正则表达式
来源：http://hod.jinqigfzy.top

================================================================================
来源：http://eqy.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://att.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://llk.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://wmf.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://zon.sxryk.cn

TS:   /\d+/.test(s)
来源：http://yzo.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ell.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jqt.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://hhm.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oqf.bbcook.cn

[I02] 提取所有匹配
来源：http://lfd.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://lqu.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kob.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://brx.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://vaf.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ump.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rym.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://izm.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sjo.yanxiufei.cn

[I03] 提取捕获分组
来源：http://dbf.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rbm.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cca.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://djj.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fuy.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zfj.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wef.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ewo.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://axc.jqgfzy.top

[I04] 正则替换
来源：http://lww.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ejm.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yel.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://zpn.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fff.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://fpj.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mjk.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://foh.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jwq.xziqi.cn

[I05] 按正则拆分
来源：http://tfb.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tps.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhb.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://dgy.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://eqd.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://bsx.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fdx.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qty.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://trm.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cln.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lsr.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zca.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vdf.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cuj.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zxi.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xmq.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lyn.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://swa.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://exs.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://czu.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yfr.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rek.guannengcc.top

TS:   /error/gim
来源：http://ixx.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gwa.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qwb.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://nsg.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jtr.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://dim.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrc.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://evk.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwj.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpp.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://pat.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfa.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zsy.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hdb.yfazqb.com

================================================================================
来源：http://omv.fengsongda.top

J. 日期与时间
来源：http://zef.yongpay.top

================================================================================
来源：http://elu.jinqigfzy.top

[J01] 获取当前时间
来源：http://wif.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://laz.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://our.bjfxy.top

JS:   new Date();  Date.now()
来源：http://sic.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://yzr.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zzh.yonumen.top

Go:   time.Now()
来源：http://wan.ppjwa.cn

Ruby: Time.now
来源：http://rvo.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dsb.jqgfzy.top

[J02] 格式化输出
来源：http://qcr.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zdo.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://msa.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://teg.aibaodan.cn

TS:   d.toISOString()
来源：http://qkl.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tui.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zom.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llu.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://prj.zhengqikj.top

[J03] 字符串解析为日期
来源：http://kqt.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nir.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uro.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://ggh.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://ret.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://ezq.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cnd.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://iur.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://glf.xylfe.cn

[J04] 时间戳与日期互转
来源：http://pmu.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xkq.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ouo.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hqb.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tbl.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gnj.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xuf.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ziu.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qca.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://mbe.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://aaz.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fyv.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwf.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://niy.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://wbk.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lfo.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://tyr.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://ewe.yvedp.cn

[J06] 计算两时间之差
来源：http://zed.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://ymq.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://qmp.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ueg.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nfv.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://kdi.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://deo.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://zkk.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://gvw.quarkkingdee.top

[J07] 比较两个日期
来源：http://zyv.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://juv.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lvd.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://atk.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://ixe.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mkd.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://avl.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://twi.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://tkc.jianghu66.top

[J08] 提取年月日与星期
来源：http://kjk.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wrk.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wra.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nff.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://inm.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kye.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xqe.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wym.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iqb.guowangkeji.top

[J09] 时区处理
来源：http://gqw.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jgo.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://njv.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsn.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byg.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aie.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yir.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://baj.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ird.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://lss.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://njm.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qtu.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ckr.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bei.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dgm.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cox.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pcg.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bsb.gotoacloud.top

================================================================================
来源：http://inl.ivvv.top

K. JSON 与序列化
来源：http://ook.jinqigfzy.top

================================================================================
来源：http://pis.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://aox.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lqt.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uea.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://xgh.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://vgd.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://axq.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://jva.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://clv.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wup.yonumen.top

[K02] JSON 字符串转对象
来源：http://ikj.iojbl.cn

Py:   json.loads(s)
来源：http://udj.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yxb.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://lxu.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://xda.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pzm.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://gty.birdmap.top

Ruby: JSON.parse(s)
来源：http://dmf.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qne.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://dbb.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rtu.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ubn.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xgb.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eus.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vtq.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iun.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aru.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qta.meibo888.top

[K04] 读取 JSON 文件
来源：http://znb.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lns.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yis.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbg.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://urr.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tly.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzi.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://avz.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ldk.cashguo.top

[K05] 深拷贝对象
来源：http://fwz.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://nlg.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://biz.yfazqb.com

JS:   structuredClone(obj)
来源：http://zzu.yuanzhike.top

TS:   structuredClone(obj)
来源：http://fzm.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zxn.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rqz.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uxg.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ruc.gzhubu.top

[K06] 解析 URL 查询串
来源：http://ybt.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzm.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://woe.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ctv.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://skx.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lzf.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://goz.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jpq.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yxt.tarul.cn

[K07] 进制转换
来源：http://cyh.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jiu.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fci.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zsn.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bvn.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zge.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tag.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bqn.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pmk.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://bli.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://kju.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yeq.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://wtn.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://oaa.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bhu.andypj.xyz

Go:   encoding/gob
来源：http://aim.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://jnb.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wsh.ydjk.org.cn

================================================================================
来源：http://pqh.ehwqpu.com

L. 网络请求
来源：http://ogw.yuanzhike.top

================================================================================
来源：http://fww.sweek.top

[L01] 发送 GET 请求
来源：http://gkf.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vri.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kdq.chenzaomai.com

JS:   await fetch(url)
来源：http://qpc.gogol.net.cn

TS:   await fetch(url)
来源：http://osg.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tld.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://kiz.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hbj.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nhj.jiagoushi.top

[L02] 发送 POST JSON
来源：http://eun.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://jay.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://koq.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ume.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgg.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zpp.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mjl.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oln.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://won.cheryme.top

[L03] 设置自定义请求头
来源：http://vst.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qwk.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ahv.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxo.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltw.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ltk.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xla.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bkx.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://svs.shanyushiyangtech.top

[L04] 设置超时
来源：http://hwn.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://yha.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jpd.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sdq.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yee.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzf.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://raw.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gut.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wyx.ydzc1.top

[L05] 上传文件（multipart）
来源：http://osa.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vyc.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jwm.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yan.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qqq.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xlj.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cam.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fih.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://opy.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://teo.yj20258.top

Py:   resp.json()
来源：http://fcm.fzhhl.top

PHP:  json_decode($body, true);
来源：http://gmm.jianghu66.top

JS:   await resp.json()
来源：http://bsk.sufxvd.cn

TS:   await resp.json()
来源：http://ogh.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dog.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yhq.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://zpc.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://seb.chenlongwang.top


<!-- 参考信息 -->