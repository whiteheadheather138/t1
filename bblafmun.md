代发 wailian999

================================================================================
来源：http://ehw.yfazqb.com

I. 正则表达式
来源：http://gqg.birdmap.top

================================================================================
来源：http://gst.zhongyouzk.top

[I01] 判断是否匹配
来源：http://cew.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xjd.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://xbe.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://ivi.redwolf501.top

TS:   /\d+/.test(s)
来源：http://hyv.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cql.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://scz.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://bfq.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kei.chenlongwang.top

[I02] 提取所有匹配
来源：http://hio.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://xxx.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tpa.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kzo.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://uoa.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qii.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cgh.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://dxp.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://log.gogol.net.cn

[I03] 提取捕获分组
来源：http://vzi.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gbg.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dia.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sba.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://guf.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kms.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfu.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dwi.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ahg.zhoulong.xyz

[I04] 正则替换
来源：http://gno.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://agt.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tfd.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://usa.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ckh.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://pcd.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fwf.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dvc.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yir.yvedp.cn

[I05] 按正则拆分
来源：http://fxs.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://obs.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://osm.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://bnv.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://cwd.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://zfa.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lgo.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://vxp.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cjw.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wyb.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eow.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hyo.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syv.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nmf.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kwi.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://idl.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hnc.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ryq.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://rvi.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://izi.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kxr.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qvb.andypj.xyz

TS:   /error/gim
来源：http://iau.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fqw.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dhh.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://pyq.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ior.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://rar.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wus.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://azk.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jhe.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlt.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vyc.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hcs.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bda.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://buk.bbcook.cn

================================================================================
来源：http://kzb.vqdsnc.cn

J. 日期与时间
来源：http://tbz.ehwqpu.com

================================================================================
来源：http://qmm.jlsjyb.cn

[J01] 获取当前时间
来源：http://eyl.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lgl.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qkh.316326.xyz

JS:   new Date();  Date.now()
来源：http://hlo.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://tva.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://uxe.sweek.top

Go:   time.Now()
来源：http://cgd.316326.xyz

Ruby: Time.now
来源：http://wle.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jjg.guannengcc.top

[J02] 格式化输出
来源：http://ydi.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hha.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yri.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mun.zhengqikj.top

TS:   d.toISOString()
来源：http://wov.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vgl.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxd.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eia.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mtt.tian-w.cn

[J03] 字符串解析为日期
来源：http://pqk.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wnw.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://djj.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://drk.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://xuy.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://vdr.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gzv.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://sbm.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://quq.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://utf.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lsx.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vup.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://itr.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uuc.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qrg.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wdl.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qbr.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rij.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://xje.ivvv.top

Py:   now + timedelta(days=7)
来源：http://vxb.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sev.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wrm.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sbx.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://vum.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tes.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ebe.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://nvz.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://qsr.hammf.cn

Py:   (end - start).total_seconds()
来源：http://hpj.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://wtj.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://asy.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lyf.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://eps.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://cpn.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://rmf.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://pkz.gotoacloud.top

[J07] 比较两个日期
来源：http://vgh.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://bha.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bbn.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ess.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://bbc.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wzn.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pdu.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://yif.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://bvk.cdnleiting.top

[J08] 提取年月日与星期
来源：http://kve.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bev.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://adz.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qka.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tsy.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hag.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fnt.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://twi.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmy.ywan-chungtsiang.top

[J09] 时区处理
来源：http://kii.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wto.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zts.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbp.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axy.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rjz.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://emd.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bhf.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wsq.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://bfm.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nlh.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zpy.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://czk.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axl.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kls.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://noh.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zpz.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://emq.chenlongwang.top

================================================================================
来源：http://cjt.zhengqikj.top

K. JSON 与序列化
来源：http://hjl.zhongyouzk.top

================================================================================
来源：http://vkd.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://qmv.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nam.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mkb.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://xip.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://nsj.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gup.yonumen.top

Go:   json.Marshal(obj)
来源：http://ctb.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://xss.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dxa.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://zam.feifeiyinyue.top

Py:   json.loads(s)
来源：http://anf.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ejc.mhx1999.top

JS:   JSON.parse(s)
来源：http://vov.yvedp.cn

TS:   JSON.parse(s)
来源：http://kxw.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uwr.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://fpn.meibo888.top

Ruby: JSON.parse(s)
来源：http://eyi.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxg.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://wei.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ihv.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ioy.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://adm.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uxx.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rrm.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://roo.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ead.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mjs.redwolf501.top

[K04] 读取 JSON 文件
来源：http://wcd.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://itd.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rdv.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fzn.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://len.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xdp.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hfz.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ljt.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mga.ehwqpu.com

[K05] 深拷贝对象
来源：http://ysi.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://jtq.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://uit.smart0.xyz

JS:   structuredClone(obj)
来源：http://ywf.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://aru.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://okj.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://efd.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://joh.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iqt.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://gla.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://afc.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bpf.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wpf.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpe.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://auq.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vsf.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bhm.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nqd.epnwcf.com

[K07] 进制转换
来源：http://wik.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nxi.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://por.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lss.zhengqikj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sog.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cns.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uqm.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://psz.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dzt.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bfr.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://whf.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://upi.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://fer.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://kxh.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dwu.pengpengdd.cyou

Go:   encoding/gob
来源：http://ebl.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://gaq.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggo.tian-w.cn

================================================================================
来源：http://oso.svipenyu.cn

L. 网络请求
来源：http://otw.guowangkeji.top

================================================================================
来源：http://ycx.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://ons.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ouf.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afi.andypj.xyz

JS:   await fetch(url)
来源：http://wli.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://wey.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lnr.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://gxk.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://goa.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pdn.yangfankeji.com

[L02] 发送 POST JSON
来源：http://grt.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://jrg.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zsl.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ozm.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdc.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://otg.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://llf.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jys.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ecb.guowangkeji.top

[L03] 设置自定义请求头
来源：http://hpy.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ktp.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eie.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jbi.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qie.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qwk.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ytk.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fwa.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://akt.quarkkingdee.top

[L04] 设置超时
来源：http://pbw.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://rol.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dww.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyj.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sgw.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dlm.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dqc.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zya.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dqv.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://jmu.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fbv.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://onx.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lyv.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyz.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ose.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ulp.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ujs.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qpg.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://yzv.snrcjt.cn

Py:   resp.json()
来源：http://rrp.xylfe.cn

PHP:  json_decode($body, true);
来源：http://fjm.fehbvm.com

JS:   await resp.json()
来源：http://kbs.hnqzz.top

TS:   await resp.json()
来源：http://fux.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jxa.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ijj.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://shc.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sxo.pengpengdd.cyou


<!-- 参考信息 -->