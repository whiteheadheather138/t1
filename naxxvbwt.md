代发 wailian999

[I02] 提取所有匹配
来源：http://fyx.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://mme.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hus.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fke.tanke756.top

TS:   s.match(/\d+/g)
来源：http://rcz.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ysr.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pou.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://ylm.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dxr.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://sdi.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jxa.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dig.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://byc.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qjw.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mwv.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://crv.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kgu.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fwv.cqqwz.cn

[I04] 正则替换
来源：http://pia.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wcm.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://viu.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://piu.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://uoc.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://jpn.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sqn.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nqh.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://khi.daria6918.cn

[I05] 按正则拆分
来源：http://lfy.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ehv.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uun.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://gle.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://psd.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://klp.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ytg.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://elj.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hbd.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qwt.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jxq.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pwi.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hrm.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovz.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://idh.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mnp.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ieo.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sbt.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://vkj.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vtx.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://due.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cyu.yfazqb.com

TS:   /error/gim
来源：http://nkx.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rhj.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://olr.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://wdj.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rlj.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://twg.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qwt.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ukm.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wca.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eyf.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aur.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fxc.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://svk.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hgf.hywenlv.cn

================================================================================
来源：http://bzl.jlsjyb.cn

J. 日期与时间
来源：http://goy.zhijiandao.cn

================================================================================
来源：http://rhc.hfpthk.cn

[J01] 获取当前时间
来源：http://cxy.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wnq.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://coj.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://xph.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://zrl.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gdm.nanxinkj.top

Go:   time.Now()
来源：http://pnv.bjfxy.top

Ruby: Time.now
来源：http://tcn.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://onh.ybcxt.top

[J02] 格式化输出
来源：http://rsv.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwz.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zqu.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nnt.havefunace.top

TS:   d.toISOString()
来源：http://xnr.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xuq.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kco.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dtq.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yvp.cqqwz.cn

[J03] 字符串解析为日期
来源：http://xmy.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ipx.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kxh.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://qlf.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://eeh.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cyi.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kqn.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rmm.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://joc.hesvh.cn

[J04] 时间戳与日期互转
来源：http://dul.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epl.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lum.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ipj.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jbw.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jxo.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zze.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfq.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fli.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://ewg.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://lup.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qog.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uen.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fek.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://ysx.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cel.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://glc.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://cjl.mhx1999.top

[J06] 计算两时间之差
来源：http://txd.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://fih.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://ffe.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cjh.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cfs.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://nmy.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://rro.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://iwr.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://hld.zhiwuduotai.top

[J07] 比较两个日期
来源：http://rax.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://omq.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://psn.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://blo.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://whh.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vuh.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fyh.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bfx.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://ggx.hcnkem.com

[J08] 提取年月日与星期
来源：http://rae.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cta.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ggj.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eez.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ant.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sas.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kgb.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsh.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lpp.smart0.xyz

[J09] 时区处理
来源：http://ota.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wyl.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fvp.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fra.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpl.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nlx.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://euv.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://att.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rno.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://vgo.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qkj.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wtx.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rfw.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fls.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pkl.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nak.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://skq.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jfs.wangshuangyany.cn

================================================================================
来源：http://uak.jlsjyb.cn

K. JSON 与序列化
来源：http://xts.hcnkem.com

================================================================================
来源：http://gra.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://czg.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uau.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mtd.hammf.cn

JS:   JSON.stringify(obj)
来源：http://xfm.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://wxp.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tih.havefunace.top

Go:   json.Marshal(obj)
来源：http://vcl.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://qib.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ydl.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://szz.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://saa.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ldx.aibaodan.cn

JS:   JSON.parse(s)
来源：http://eeh.sweek.top

TS:   JSON.parse(s)
来源：http://sth.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tyk.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://mra.guannengcc.top

Ruby: JSON.parse(s)
来源：http://geq.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zgv.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://kkc.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gcm.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xwh.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ibu.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fxu.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://igl.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pqu.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://okg.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vlt.sweek.top

[K04] 读取 JSON 文件
来源：http://vaj.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wvz.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://new.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gce.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wmv.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ino.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://scq.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://gav.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rjk.yonumen.top

[K05] 深拷贝对象
来源：http://ghx.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://irb.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://bpx.jqgfzy.top

JS:   structuredClone(obj)
来源：http://rno.tian-w.cn

TS:   structuredClone(obj)
来源：http://ljt.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://nda.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://obq.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xok.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zfk.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://fls.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://def.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dep.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbi.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yps.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bal.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ijx.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yht.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsj.shangyingyoupin.top

[K07] 进制转换
来源：http://yvf.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ian.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gwa.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iit.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dbo.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://des.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fvd.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qus.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://arj.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://bpo.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://xud.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rkf.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://enq.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://vjt.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ppb.nwbrower.top

Go:   encoding/gob
来源：http://qzq.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://qds.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qan.fanxiaobao.xyz

================================================================================
来源：http://dbh.yj20258.top

L. 网络请求
来源：http://ypp.xingfuxueyuan.xyz

================================================================================
来源：http://awr.aibaodan.cn

[L01] 发送 GET 请求
来源：http://cuf.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dbv.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tjm.smart0.xyz

JS:   await fetch(url)
来源：http://gkm.gaohongyu789.top

TS:   await fetch(url)
来源：http://qbg.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mai.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://eaf.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lyf.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pnn.zycfv.cn

[L02] 发送 POST JSON
来源：http://pxk.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://xmy.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ypr.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ciu.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwc.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uag.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fvt.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://num.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mpr.yuxming.cn

[L03] 设置自定义请求头
来源：http://ubc.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nuz.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wkq.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdq.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvg.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hct.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mlm.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://djv.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ztt.zdqjudy.top

[L04] 设置超时
来源：http://dzr.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://oiq.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cre.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://psl.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zgo.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://spv.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mfc.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zgj.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xdc.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://gqn.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dew.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xzb.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzp.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://whz.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbd.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ago.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wrc.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vax.yueranfly.top

[L06] 解析响应为 JSON
来源：http://frw.andypj.xyz

Py:   resp.json()
来源：http://iax.sxryk.cn

PHP:  json_decode($body, true);
来源：http://lkr.fzhhl.top

JS:   await resp.json()
来源：http://orb.yj202588.top

TS:   await resp.json()
来源：http://hgf.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tjy.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fxs.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://tir.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kja.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://wxd.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://feq.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://inx.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://srd.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://tmm.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://avh.yfazqb.com

Go:   resp.StatusCode
来源：http://lim.xylfe.cn

Ruby: resp.code.to_i
来源：http://xzf.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://kkn.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://nzw.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lem.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://nzi.bbcook.cn


<!-- 参考信息 -->