代发 wailian999

[I02] 提取所有匹配
来源：http://lkt.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://pzi.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lsd.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nns.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://giq.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lhp.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xyg.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://jwu.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ttu.yj20258888.top

[I03] 提取捕获分组
来源：http://uof.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://omv.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tbi.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sfk.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ijj.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://viv.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vhp.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jaq.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://unh.jinghuilouyu.cn

[I04] 正则替换
来源：http://uzy.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lze.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://elm.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lcx.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://sxa.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ffn.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ouq.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gxf.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://osd.52xcode.cn

[I05] 按正则拆分
来源：http://slu.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uxa.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tgb.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://rbp.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://fwk.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://eus.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rmb.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://lwv.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pfo.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ojc.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uuu.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ljl.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebe.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pil.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uvz.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lbc.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://use.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bgb.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://wmi.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xpq.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jjs.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mcv.kuanghao11.cn

TS:   /error/gim
来源：http://awm.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zei.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rna.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://agz.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://llj.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://adc.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nem.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amy.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://koi.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqe.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgc.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wry.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://upz.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hql.chenlongwang.top

================================================================================
来源：http://fui.meibo888.top

J. 日期与时间
来源：http://hmv.0kj1m.cn

================================================================================
来源：http://goe.bbcook.cn

[J01] 获取当前时间
来源：http://ntj.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rca.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pkx.havefunace.top

JS:   new Date();  Date.now()
来源：http://cvq.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://zfj.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kgq.jinqigufen.top

Go:   time.Now()
来源：http://njh.pengpengdd.cyou

Ruby: Time.now
来源：http://uxd.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wdg.zdqjudy.top

[J02] 格式化输出
来源：http://ocp.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://paj.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vzc.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yku.52xcode.cn

TS:   d.toISOString()
来源：http://asa.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ruw.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fje.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iwv.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pxa.sweek.top

[J03] 字符串解析为日期
来源：http://qbf.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fkd.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bxj.hammf.cn

JS:   new Date("2024-01-02")
来源：http://kpb.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://tcv.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://edr.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kth.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://eza.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rjn.tanke756.top

[J04] 时间戳与日期互转
来源：http://kng.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gka.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdj.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kae.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qwd.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fqr.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fku.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cnc.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mir.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://jmd.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://hrf.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://feh.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvl.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gng.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://kfb.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssp.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://dkp.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yfo.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://pys.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://sfr.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://opp.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://znw.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vvb.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ium.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://ppb.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://cyy.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://vzq.jyoumei.cn

[J07] 比较两个日期
来源：http://xlk.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://ckc.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lcb.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://msc.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://yaa.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pix.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://opw.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://ddp.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://lro.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://ogx.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://njy.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ziz.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oji.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://afp.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pis.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://flx.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ngh.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ozm.fehbvm.com

[J09] 时区处理
来源：http://fvk.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://riw.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ias.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://muq.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyz.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bxi.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bpt.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cby.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mzs.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://qcc.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kzn.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iku.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://obj.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nuu.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ajt.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kgg.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oxg.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://quk.sysykeji.top

================================================================================
来源：http://ese.shuidangran.top

K. JSON 与序列化
来源：http://fsa.yj20258888.top

================================================================================
来源：http://rfn.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://kzv.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iil.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rhb.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://gio.cheryme.top

TS:   JSON.stringify(obj)
来源：http://vth.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nox.smart0.xyz

Go:   json.Marshal(obj)
来源：http://qwu.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://uxt.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nlf.yueranfly.top

[K02] JSON 字符串转对象
来源：http://ati.yuxming.cn

Py:   json.loads(s)
来源：http://iyx.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://muk.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://hob.cashguo.top

TS:   JSON.parse(s)
来源：http://fsd.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aeo.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://qxi.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://asz.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bof.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://num.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ong.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gce.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gge.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yhg.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wur.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hzo.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://llf.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hal.yj20258888.top

[K04] 读取 JSON 文件
来源：http://kfo.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kkd.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ein.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zqs.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mao.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nnv.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbo.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cqt.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oxh.jinqigfzy.top

[K05] 深拷贝对象
来源：http://juq.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://xet.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://wpg.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://bqc.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://ahq.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tta.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gnu.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tij.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pvm.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://caz.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mok.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ofy.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txs.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hnm.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxk.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hkc.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ggh.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://agr.zhengqikj.top

[K07] 进制转换
来源：http://sis.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zff.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bjp.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kjb.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cgw.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsf.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nvd.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://abw.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xly.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://pza.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://frj.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gax.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://vqa.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://iwr.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://llf.zdbjq.cn

Go:   encoding/gob
来源：http://hss.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://oqh.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://myr.yangfankeji.com

================================================================================
来源：http://rpa.hfpthk.cn

L. 网络请求
来源：http://bgg.zdbjq.cn

================================================================================
来源：http://qlc.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://acj.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qhg.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lvo.cqqwz.cn

JS:   await fetch(url)
来源：http://tzq.xuanzx.com

TS:   await fetch(url)
来源：http://czr.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uhq.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://zbq.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bxf.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jui.ctjpmb.com

[L02] 发送 POST JSON
来源：http://ony.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://fvr.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ecm.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zda.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jes.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://les.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lbi.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pwd.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://psy.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://trj.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://amq.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lcu.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://txv.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gye.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cka.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bfo.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qte.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xzz.jinyuanbaomall.cn

[L04] 设置超时
来源：http://pgl.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://zbr.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nzb.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmu.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdx.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ats.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cib.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aoi.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rts.pycfn.com

[L05] 上传文件（multipart）
来源：http://ajx.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fsg.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dwe.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bnb.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vqi.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ypf.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yck.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cfu.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cpo.sxryk.cn

[L06] 解析响应为 JSON
来源：http://ejm.jqgfzy.top

Py:   resp.json()
来源：http://trf.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://ini.hysaishi.cn

JS:   await resp.json()
来源：http://wtz.52xcode.cn

TS:   await resp.json()
来源：http://sji.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vie.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hdd.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://ayt.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xlu.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://sym.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ulv.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wqh.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://jmo.cashguo.top

TS:   resp.ok;  resp.status
来源：http://rdy.vehdjk.com

Java: resp.statusCode()
来源：http://mts.zhixingplan.top

Go:   resp.StatusCode
来源：http://pym.ivvv.top

Ruby: resp.code.to_i
来源：http://roi.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://qyk.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://wzo.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://igr.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://rbd.hysaishi.cn


<!-- 参考信息 -->