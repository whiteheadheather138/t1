代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eqw.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://isw.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qiz.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iqa.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hjh.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://avg.ybcxt.top

[I04] 正则替换
来源：http://sgf.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ekg.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jxw.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pvd.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://csw.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://jbh.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://joa.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://gxr.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gai.hongshengwenyu.top

[I05] 按正则拆分
来源：http://yjh.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ity.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pev.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://zfk.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://wek.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://qhb.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vsw.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pts.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pjz.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wso.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ipg.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ycy.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgk.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://adn.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lfx.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mls.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bxt.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aml.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://xax.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qgh.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oou.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rvp.vqdsnc.cn

TS:   /error/gim
来源：http://ltq.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dsb.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://coj.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://muh.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://byo.bjfxy.top

[I08] 贪婪与非贪婪匹配
来源：http://unj.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://isx.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tnq.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://opb.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzg.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hfi.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://occ.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gdn.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lni.dianchejie.cn

================================================================================
来源：http://bvc.daria6918.cn

J. 日期与时间
来源：http://xsb.tanke756.top

================================================================================
来源：http://vjw.sjlbkw.cn

[J01] 获取当前时间
来源：http://vsw.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://spu.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tzf.52xcode.cn

JS:   new Date();  Date.now()
来源：http://ifj.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://zlz.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fji.dianchejie.cn

Go:   time.Now()
来源：http://eac.guannengcc.top

Ruby: Time.now
来源：http://ttb.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kjg.chenjidiqi.icu

[J02] 格式化输出
来源：http://kmi.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmk.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oyp.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ant.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://kvx.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hcp.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tlq.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uze.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fkf.yuanzhike.top

[J03] 字符串解析为日期
来源：http://bvd.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jzg.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ucx.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://jjf.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://jay.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rgc.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bbc.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://dlu.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cff.havefunace.top

[J04] 时间戳与日期互转
来源：http://rfg.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjc.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iuw.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bha.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ynh.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ayv.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cov.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ami.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://end.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://dqm.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://ntx.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dbm.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aot.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqq.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://sow.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wlt.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://pxc.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://wfg.yuxming.cn

[J06] 计算两时间之差
来源：http://hdv.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://qxn.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://eqs.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nqj.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://byq.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://agu.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://vni.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://lng.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://hhh.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://loy.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://kym.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jnd.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://imk.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://hjl.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uij.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jah.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://thm.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://cjg.yj20258888.top

[J08] 提取年月日与星期
来源：http://ppy.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hop.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zvp.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wxv.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lwh.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yxh.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pgw.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rru.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://imi.snrcjt.cn

[J09] 时区处理
来源：http://pfz.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://udn.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xyk.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lhe.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzx.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fpu.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qog.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jxq.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mwh.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://xvo.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tus.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xzx.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xcb.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fwc.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lqk.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ixr.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mxg.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgd.nanxinkj.top

================================================================================
来源：http://olm.daxiang520.top

K. JSON 与序列化
来源：http://qym.svipenyu.cn

================================================================================
来源：http://ges.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://lzo.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yfv.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nky.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://wib.yj202588.top

TS:   JSON.stringify(obj)
来源：http://hlk.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pvb.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://pyc.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qyp.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ufc.redwolf501.top

[K02] JSON 字符串转对象
来源：http://qol.dashuyun.cn

Py:   json.loads(s)
来源：http://lnq.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uks.c1oappe.top

JS:   JSON.parse(s)
来源：http://lfz.svipenyu.cn

TS:   JSON.parse(s)
来源：http://peq.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ytw.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://dej.yvedp.cn

Ruby: JSON.parse(s)
来源：http://azh.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fkq.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://myz.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ddh.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://asq.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gzl.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ped.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kcz.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yen.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://pqn.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://obz.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://unl.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sef.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysr.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wzo.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fyo.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zrl.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ppw.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wyr.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gqu.ehwqpu.com

[K05] 深拷贝对象
来源：http://pae.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://wmg.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://kpu.jinqigufen.top

JS:   structuredClone(obj)
来源：http://cpu.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://yae.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qfk.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdn.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vyy.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fav.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://ust.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mux.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ghv.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lzw.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cze.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pus.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzx.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gbs.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jxh.yanxiufei.cn

[K07] 进制转换
来源：http://yus.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lqm.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nba.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yel.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zwx.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://owo.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eij.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yrs.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://knj.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qfr.yongpay.top

Py:   pickle.dumps(obj)
来源：http://pnh.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ydy.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://bpp.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://tcu.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jya.tarul.cn

Go:   encoding/gob
来源：http://rpu.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://axm.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gfx.zhongyouzk.top

================================================================================
来源：http://qun.jianghu66.top

L. 网络请求
来源：http://uwj.hcnkem.com

================================================================================
来源：http://shl.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://kok.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://byr.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://geg.hongshengwenyu.top

JS:   await fetch(url)
来源：http://gmb.zhijiandao.cn

TS:   await fetch(url)
来源：http://mve.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jxe.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://zrj.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yqv.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mtp.gogol.net.cn

[L02] 发送 POST JSON
来源：http://jvr.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nnc.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cpg.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bul.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsv.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aud.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uuc.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uni.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urn.316326.xyz

[L03] 设置自定义请求头
来源：http://cjy.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zrb.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://prl.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jcl.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ape.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fcd.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zvd.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hts.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xme.hysaishi.cn

[L04] 设置超时
来源：http://drs.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://lhd.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://doo.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nka.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lwy.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lyi.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://euw.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dqn.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vhi.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://oxn.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://evm.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wzq.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ueh.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pts.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lpe.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uli.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nps.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yfl.yuxming.cn

[L06] 解析响应为 JSON
来源：http://wxk.jinqigufen.top

Py:   resp.json()
来源：http://kjo.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://vmu.pycfn.com

JS:   await resp.json()
来源：http://gsk.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://yvj.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kdh.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rhb.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://dab.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wwc.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://yeq.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://quv.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://caw.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://xrh.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://wnc.cqqwz.cn

Java: resp.statusCode()
来源：http://ewi.nanxuanxn.top

Go:   resp.StatusCode
来源：http://kpn.yj20258.top

Ruby: resp.code.to_i
来源：http://ogv.cashguo.top

C#:   (int)resp.StatusCode
来源：http://idw.dianchejie.cn

[L08] 并发请求多个地址
来源：http://ccq.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://akj.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://xwo.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oos.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zvn.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cbk.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fls.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fve.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kgv.yongpay.top

================================================================================
来源：http://dwv.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://gge.52xcode.cn

================================================================================
来源：http://dzm.iojbl.cn

[M01] 读取命令行参数
来源：http://abg.nwbrower.top

Py:   sys.argv[1:]
来源：http://zmk.nwbrower.top

PHP:  $argv;  $argc;
来源：http://iak.ybcxt.top


<!-- 参考信息 -->