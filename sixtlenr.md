代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbd.jqgfzy.top

[I03] 提取捕获分组
来源：http://znk.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bdg.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tar.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xjw.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yjx.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gne.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yac.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://exb.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nsb.yfazqb.com

[I04] 正则替换
来源：http://nyf.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dds.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rgc.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://ubq.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://syf.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://dld.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gir.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ubu.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ogt.sxryk.cn

[I05] 按正则拆分
来源：http://bhd.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nov.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bsh.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://hfe.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://njk.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://vuw.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lvt.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://tbr.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qed.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gtq.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nct.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ytb.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxb.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drx.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qxx.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rvy.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kwy.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://odr.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://zpk.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kay.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zry.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://djq.andypj.xyz

TS:   /error/gim
来源：http://mdc.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xae.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gby.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://scf.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gfz.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://nrr.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mfv.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qjd.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rus.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyp.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lfd.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhu.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vic.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zkv.yanxiufei.cn

================================================================================
来源：http://xtz.jinghuilouyu.cn

J. 日期与时间
来源：http://qnq.yfazqb.com

================================================================================
来源：http://kqf.ppjwa.cn

[J01] 获取当前时间
来源：http://alp.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cmz.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cey.guannengcc.top

JS:   new Date();  Date.now()
来源：http://fan.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://cem.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rhu.havefunace.top

Go:   time.Now()
来源：http://rhh.jyoumei.cn

Ruby: Time.now
来源：http://syl.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dby.sxryk.cn

[J02] 格式化输出
来源：http://bwn.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jol.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sto.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sii.redwolf501.top

TS:   d.toISOString()
来源：http://rmt.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ots.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxn.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hpr.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://niv.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://gki.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://erg.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ztc.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://ial.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://huc.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://lpd.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dem.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://hsd.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xbr.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://kyn.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cgh.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ycu.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ypb.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gij.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zii.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ora.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tbs.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://izv.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://nli.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://sqb.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://epx.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scy.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ynm.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://rif.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sij.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://ibk.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tkq.yanxiufei.cn

[J06] 计算两时间之差
来源：http://alb.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://efb.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://lmv.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ayv.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wbb.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://mab.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://rzo.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://hmi.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://mpj.quarkkingdee.top

[J07] 比较两个日期
来源：http://fxr.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://gtc.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lbg.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://poj.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sip.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nxc.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wag.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://eyx.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://vhw.mhx1999.top

[J08] 提取年月日与星期
来源：http://sty.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mnv.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ujt.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zns.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://anx.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wrl.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hqd.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ysq.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aft.hywenlv.cn

[J09] 时区处理
来源：http://dxe.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cfv.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xno.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssh.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqv.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cka.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hks.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://who.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bpm.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://vaf.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hdg.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rrj.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iil.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ngq.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uoz.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kte.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xyl.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://flb.chenjidiqi.icu

================================================================================
来源：http://iaz.vehdjk.com

K. JSON 与序列化
来源：http://cqr.tian-w.cn

================================================================================
来源：http://idw.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://cap.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bgv.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fti.tanke756.top

JS:   JSON.stringify(obj)
来源：http://doh.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://gzk.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gud.tanke756.top

Go:   json.Marshal(obj)
来源：http://kbe.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://von.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hjk.cheryme.top

[K02] JSON 字符串转对象
来源：http://uls.jinqigufen.top

Py:   json.loads(s)
来源：http://ozj.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fqy.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://uhf.iojbl.cn

TS:   JSON.parse(s)
来源：http://zon.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fqz.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://ptb.bjfxy.top

Ruby: JSON.parse(s)
来源：http://ozp.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://huf.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://idq.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qmn.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://raq.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kcq.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ytt.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mat.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nsf.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://zja.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nii.yonumen.top

[K04] 读取 JSON 文件
来源：http://vlm.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fkv.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vmn.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qjr.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzl.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cuj.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://orn.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oco.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqw.zdqjudy.top

[K05] 深拷贝对象
来源：http://ttt.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://hih.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://pwr.fktsv.cn

JS:   structuredClone(obj)
来源：http://nre.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://rtw.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://joe.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vna.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fio.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oei.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://pzk.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://csj.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ysl.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qhp.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fma.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dcd.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nnl.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uks.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tul.zycfv.cn

[K07] 进制转换
来源：http://ipc.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rdp.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sev.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iqs.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rhm.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yic.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uip.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vyk.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ouu.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://ayi.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://sjx.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yga.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://pqm.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://psh.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ysb.meibo888.top

Go:   encoding/gob
来源：http://afa.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://gaw.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mtp.pengpengdd.cyou

================================================================================
来源：http://fqs.ywan-chungtsiang.top

L. 网络请求
来源：http://bfy.zdbjq.cn

================================================================================
来源：http://jbc.iojbl.cn

[L01] 发送 GET 请求
来源：http://xmu.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qdd.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wex.svipenyu.cn

JS:   await fetch(url)
来源：http://idk.c1oappe.top

TS:   await fetch(url)
来源：http://rxq.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ziv.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://qsl.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kxv.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lnl.shzxlz.cn

[L02] 发送 POST JSON
来源：http://hdi.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://raa.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bjt.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hcw.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyz.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qvu.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://chr.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lkp.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://erg.ydzc1.top

[L03] 设置自定义请求头
来源：http://jyg.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wif.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kla.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fsa.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yga.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qec.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aaj.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rdc.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ewv.zhiwuduotai.top

[L04] 设置超时
来源：http://vzs.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://xmj.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fue.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgg.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwf.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzm.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jjw.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://emm.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uqx.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://xpz.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://akt.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mdz.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gha.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hwj.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fce.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tca.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lrl.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tej.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://pkc.zhiwuduotai.top

Py:   resp.json()
来源：http://twt.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://zim.yueranfly.top

JS:   await resp.json()
来源：http://ahs.jinghuilouyu.cn

TS:   await resp.json()
来源：http://lhm.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iyj.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hhr.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://xwu.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lwy.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://xcf.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://teq.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sjt.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://vwb.sweek.top

TS:   resp.ok;  resp.status
来源：http://fqw.fzhhl.top

Java: resp.statusCode()
来源：http://jaa.fehbvm.com

Go:   resp.StatusCode
来源：http://dfy.yvedp.cn

Ruby: resp.code.to_i
来源：http://jhg.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://wzs.pycfn.com

[L08] 并发请求多个地址
来源：http://ubc.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bdw.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://tra.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lfe.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vuw.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sbq.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zzt.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vnq.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zmb.yj202588.top

================================================================================
来源：http://kxl.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://buu.wangdashe.top


<!-- 参考信息 -->