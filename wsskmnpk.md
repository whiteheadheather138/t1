代发 wailian999

[I02] 提取所有匹配
来源：http://gyo.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://tmj.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ppm.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ejv.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://saj.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qpr.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pmp.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://fzi.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rdt.gzhubu.top

[I03] 提取捕获分组
来源：http://wkn.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oew.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yeq.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oey.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hnn.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wld.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ahq.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bpv.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tpd.jinqigfzy.top

[I04] 正则替换
来源：http://cdb.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ybd.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kjy.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://vkd.shuidangran.top

TS:   s.replace(/\d+/g, "#")
来源：http://qye.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ayb.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wkf.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://khq.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yep.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://dzu.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iwr.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hia.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://sxk.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://ymt.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://ynf.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sdg.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xeh.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bec.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://thp.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nmm.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oat.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ier.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hyt.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jel.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://btt.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hvs.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lgj.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://ftt.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wob.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aet.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://are.xziqi.cn

TS:   /error/gim
来源：http://yvq.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qgx.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zdq.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://xpa.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lad.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://ycw.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sau.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://byl.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uja.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://psw.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wak.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://luk.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hdv.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gzb.jqgfzy.top

================================================================================
来源：http://qtb.xuanzx.com

J. 日期与时间
来源：http://gtr.hammf.cn

================================================================================
来源：http://zas.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://xqn.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kqk.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://shc.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://bqa.shuidangran.top

TS:   new Date();  Date.now()
来源：http://bqf.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://upc.pengpengdd.cyou

Go:   time.Now()
来源：http://axq.hnxiangtu.top

Ruby: Time.now
来源：http://aop.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zun.quarkkingdee.top

[J02] 格式化输出
来源：http://tkn.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gwn.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dsv.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lln.chenzaomai.com

TS:   d.toISOString()
来源：http://vuh.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pvj.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nxg.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gbc.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rtl.yj20258888.top

[J03] 字符串解析为日期
来源：http://gby.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sdr.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wub.redwolf501.top

JS:   new Date("2024-01-02")
来源：http://oto.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://pla.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://hcc.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fqs.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://dqj.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jmc.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://ulr.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sgl.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ojd.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tid.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lan.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cdu.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tem.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tmp.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baw.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://kfb.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://eua.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iur.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qlo.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgy.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://gmr.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wzy.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://osx.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://mos.kuanghao11.cn

[J06] 计算两时间之差
来源：http://kos.pycfn.com

Py:   (end - start).total_seconds()
来源：http://bda.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://kng.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jzz.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cnc.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://ozs.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://wya.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://ath.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://ubo.haohaochexian.top

[J07] 比较两个日期
来源：http://jbo.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://jpg.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://idi.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://nfz.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://sou.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fga.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wen.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hyp.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://kvh.yj202588.top

[J08] 提取年月日与星期
来源：http://vry.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tgi.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbj.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qpv.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uss.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://piu.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tea.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kzk.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ead.0kj1m.cn

[J09] 时区处理
来源：http://kfv.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jti.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bdf.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gir.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gyc.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lfs.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ctx.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hbc.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wuq.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://enu.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://yhx.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ggo.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdg.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qnk.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hub.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://frj.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hsv.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hee.tianlin.xyz

================================================================================
来源：http://cnn.ehwqpu.com

K. JSON 与序列化
来源：http://pvq.yuxming.cn

================================================================================
来源：http://jhs.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://dby.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qen.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rcm.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://uuy.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://fbb.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xiw.sweek.top

Go:   json.Marshal(obj)
来源：http://cft.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qna.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yof.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://abj.yueranfly.top

Py:   json.loads(s)
来源：http://noh.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ata.chenzaomai.com

JS:   JSON.parse(s)
来源：http://lgt.guowangkeji.top

TS:   JSON.parse(s)
来源：http://hej.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wyw.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://rrc.guannengcc.top

Ruby: JSON.parse(s)
来源：http://oig.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wzx.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://xrl.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iad.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ewx.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://kod.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hjw.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xek.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ekr.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://gkl.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mrn.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://kop.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dzb.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fek.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qdd.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://alp.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ivl.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tkv.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rjl.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yjv.zhengqikj.top

[K05] 深拷贝对象
来源：http://smm.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://qiw.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://dpc.smart0.xyz

JS:   structuredClone(obj)
来源：http://plw.tarul.cn

TS:   structuredClone(obj)
来源：http://cvn.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://imx.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pon.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yvq.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hom.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://wbt.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fzj.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tbx.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asa.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ibd.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qrc.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bnj.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mih.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://miy.haohaochexian.top

[K07] 进制转换
来源：http://kam.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qjm.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dat.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://puv.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ydy.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://usc.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fpq.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oas.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rls.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://rim.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://mcn.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://agp.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://edf.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://jed.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sfq.chenzaomai.com

Go:   encoding/gob
来源：http://mbg.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://xtl.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nbw.gaohongyu789.top

================================================================================
来源：http://hmo.mhx1999.top

L. 网络请求
来源：http://oqz.zhaomingkeji.xyz

================================================================================
来源：http://fbm.jinqigufen.top

[L01] 发送 GET 请求
来源：http://dlb.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ijw.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nsg.zycfv.cn

JS:   await fetch(url)
来源：http://egr.tarul.cn

TS:   await fetch(url)
来源：http://rtv.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qcm.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://vdz.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xyl.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://msg.316326.xyz

[L02] 发送 POST JSON
来源：http://btn.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://ooz.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ibm.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ubb.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cea.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zkj.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://haq.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dgz.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xfv.jyoumei.cn

[L03] 设置自定义请求头
来源：http://lge.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xng.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hdx.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rul.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rrv.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ljz.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lcc.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gzr.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkq.sxryk.cn

[L04] 设置超时
来源：http://cbe.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://sxi.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bux.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwi.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lxn.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://axr.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ite.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upd.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yac.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://wpf.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bri.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lfy.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://znx.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ffk.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yia.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yyh.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lfy.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zep.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://gme.uphjek.com

Py:   resp.json()
来源：http://khl.cashguo.top

PHP:  json_decode($body, true);
来源：http://ijs.316326.xyz

JS:   await resp.json()
来源：http://xji.chenjidiqi.icu

TS:   await resp.json()
来源：http://yms.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ejy.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kje.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://hpp.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ucj.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://zqe.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ikc.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sht.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://hws.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://lfn.dashuyun.cn

Java: resp.statusCode()
来源：http://vrk.fengsongda.top

Go:   resp.StatusCode
来源：http://jlv.tanke756.top

Ruby: resp.code.to_i
来源：http://oqi.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://zym.gzhubu.top

[L08] 并发请求多个地址
来源：http://jxe.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ull.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://ita.svipenyu.cn


<!-- 参考信息 -->