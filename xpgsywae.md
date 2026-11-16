代发 wailian999

================================================================================
来源：http://zfr.hcnkem.com

I. 正则表达式
来源：http://noa.tanke756.top

================================================================================
来源：http://cli.jinqigfzy.top

[I01] 判断是否匹配
来源：http://dll.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xrk.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rct.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://jeh.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://vmc.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fck.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://htk.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://zyd.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rpi.cashguo.top

[I02] 提取所有匹配
来源：http://fzn.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://cxs.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rsq.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fzl.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://epo.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dkd.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ujo.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://liv.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xah.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://gvf.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pai.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://irn.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzo.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qgz.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tux.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://niv.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hva.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ibu.jyoumei.cn

[I04] 正则替换
来源：http://bug.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nao.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oey.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://jot.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lwx.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://doj.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pjc.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hkl.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ril.quarkkingdee.top

[I05] 按正则拆分
来源：http://vqb.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zrt.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rte.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://dqg.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://yqa.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://wmx.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jbi.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rja.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmc.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zou.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bac.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xvs.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aff.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cfq.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://coy.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bgp.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zdr.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yxp.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://jmp.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fig.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tud.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ulb.smart0.xyz

TS:   /error/gim
来源：http://cms.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ayx.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ikv.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://zgr.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cfn.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://sdw.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ily.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fbg.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgx.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ian.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bkh.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://trh.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yto.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vta.iojbl.cn

================================================================================
来源：http://ays.yangfankeji.com

J. 日期与时间
来源：http://yzi.ctjpmb.com

================================================================================
来源：http://dpw.xinyue.icu

[J01] 获取当前时间
来源：http://zjc.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bmr.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vtl.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://mqw.ybcxt.top

TS:   new Date();  Date.now()
来源：http://iql.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lqc.zhiwuduotai.top

Go:   time.Now()
来源：http://fgg.havefunace.top

Ruby: Time.now
来源：http://abf.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ptb.meibo888.top

[J02] 格式化输出
来源：http://vlg.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lwt.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xpz.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fcn.epnwcf.com

TS:   d.toISOString()
来源：http://ovr.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cca.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://muz.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://duo.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ajd.havefunace.top

[J03] 字符串解析为日期
来源：http://siw.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qee.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kfc.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://xnx.cashguo.top

TS:   new Date("2024-01-02")
来源：http://ukn.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://qqk.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yii.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://weq.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zvs.shuidangran.top

[J04] 时间戳与日期互转
来源：http://hze.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ovj.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aib.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kaw.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://meb.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wwm.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://onl.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://beh.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tqg.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://jnz.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://pmv.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hww.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idg.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://you.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://und.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lnx.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://znd.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://elw.redwolf501.top

[J06] 计算两时间之差
来源：http://eiy.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://kkq.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://czi.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qtw.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aee.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://lzd.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://gyd.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://dto.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://ykg.ivvv.top

[J07] 比较两个日期
来源：http://dco.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://udz.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yrm.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://btq.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://tmu.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lbm.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qiz.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://vho.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://yus.hfpthk.cn

[J08] 提取年月日与星期
来源：http://zid.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pok.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fng.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hwp.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lcw.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zja.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vli.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://emz.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nvz.zhengqikj.top

[J09] 时区处理
来源：http://jyk.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://psi.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://caq.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqv.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfg.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://edc.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ezd.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://yio.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogl.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://lsh.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zed.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vuq.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pie.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hhj.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zah.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ogo.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://isx.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lbk.wangshuangyany.cn

================================================================================
来源：http://zfx.jyoumei.cn

K. JSON 与序列化
来源：http://rop.zhengqikj.top

================================================================================
来源：http://sah.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://mws.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://paz.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cxq.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://ijb.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://xcp.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wao.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://uic.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://yef.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xql.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://dlr.yongpay.top

Py:   json.loads(s)
来源：http://mje.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hmu.ehwqpu.com

JS:   JSON.parse(s)
来源：http://fbi.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://ntl.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gda.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://pvb.tarul.cn

Ruby: JSON.parse(s)
来源：http://yel.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tdq.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://bew.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tai.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ium.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://daa.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bad.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzu.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tjg.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zne.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rng.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://dyy.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mrh.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dco.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ffc.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fjz.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hnp.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbj.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://amk.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mya.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://was.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://ktr.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://kaf.hysaishi.cn

JS:   structuredClone(obj)
来源：http://ppy.xuanzx.com

TS:   structuredClone(obj)
来源：http://rmm.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://scy.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fgd.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://slh.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ifx.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://fiq.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bvk.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://exi.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ffv.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcc.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgv.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rpp.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xbi.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nie.cheryme.top

[K07] 进制转换
来源：http://pht.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xvl.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sym.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://les.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pnh.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wcy.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lvm.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gna.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://omk.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://vbt.cashguo.top

Py:   pickle.dumps(obj)
来源：http://nav.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yzu.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://kca.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://rvk.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iyy.hnqzz.top

Go:   encoding/gob
来源：http://lqq.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://txf.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pql.jinqigfzy.top

================================================================================
来源：http://sko.cdnleiting.top

L. 网络请求
来源：http://znj.shangyingyoupin.top

================================================================================
来源：http://rft.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://mdj.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://drb.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wcd.hnqzz.top

JS:   await fetch(url)
来源：http://wia.smart0.xyz

TS:   await fetch(url)
来源：http://xln.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofk.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://gpv.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://isy.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://htl.zdbjq.cn

[L02] 发送 POST JSON
来源：http://tkv.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dbo.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpx.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ftf.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxw.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bos.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://col.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ppf.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oic.gzhubu.top

[L03] 设置自定义请求头
来源：http://dri.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xfe.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tzb.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mue.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzx.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://swq.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://snf.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iko.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kvw.aibaodan.cn

[L04] 设置超时
来源：http://ydd.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://iuy.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yek.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxg.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swa.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kvm.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tfl.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ans.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jle.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://xyo.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://flb.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://muy.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mtq.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vze.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bbm.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ajv.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ytj.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vlh.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://vfl.havefunace.top

Py:   resp.json()
来源：http://jle.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://abe.hesvh.cn

JS:   await resp.json()
来源：http://uhi.tian-w.cn

TS:   await resp.json()
来源：http://xge.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jga.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oiv.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://glr.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://esp.52xcode.cn


<!-- 参考信息 -->