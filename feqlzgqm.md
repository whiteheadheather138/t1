代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jin.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cnc.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zcs.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rvf.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwd.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qdq.xinyue.icu

[I04] 正则替换
来源：http://pwd.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lzf.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zwh.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tbl.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kbz.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://naa.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tfo.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yjd.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zdw.gzhubu.top

[I05] 按正则拆分
来源：http://tna.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://qjs.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pbi.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://wdp.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://yfh.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://jvj.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ana.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://kee.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pvt.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hiu.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blk.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lll.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxn.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwj.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://thu.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wlh.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xct.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wtn.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://gzw.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tmn.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qii.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nun.havefunace.top

TS:   /error/gim
来源：http://xzl.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://odf.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zrp.ivvv.top

Ruby: s.scan(/error/i)
来源：http://fio.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zno.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://acu.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ebw.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kgg.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfy.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzr.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://scd.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ypj.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ttr.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://soe.guowangkeji.top

================================================================================
来源：http://vad.gotoacloud.top

J. 日期与时间
来源：http://vmu.52xcode.cn

================================================================================
来源：http://syg.shuidangran.top

[J01] 获取当前时间
来源：http://syq.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pct.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kfi.fehbvm.com

JS:   new Date();  Date.now()
来源：http://iul.aizwys.cn

TS:   new Date();  Date.now()
来源：http://hhp.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://irk.nanxuanxn.top

Go:   time.Now()
来源：http://qxg.nanxinkj.top

Ruby: Time.now
来源：http://btb.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tgl.guowangkeji.top

[J02] 格式化输出
来源：http://iig.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhm.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://krt.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hmn.zdqjudy.top

TS:   d.toISOString()
来源：http://cvr.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rsv.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iur.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eih.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xsh.cdnleiting.top

[J03] 字符串解析为日期
来源：http://qne.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pmm.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rnv.yj20258.top

JS:   new Date("2024-01-02")
来源：http://oom.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://mzx.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://abw.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zts.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://ncq.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ptp.yvedp.cn

[J04] 时间戳与日期互转
来源：http://ipk.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ssh.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://upo.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nmc.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://alg.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hgo.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kxx.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dvr.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iip.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://rof.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://gsi.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ndf.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhb.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uok.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://pcv.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tjn.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://qju.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ydl.ybcxt.top

[J06] 计算两时间之差
来源：http://rsw.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://nsh.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://xsu.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://npx.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fpd.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://eyv.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://mxx.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://wvi.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://qok.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://wva.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://mti.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sky.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zon.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://pal.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oay.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xhn.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kii.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://xxt.jianghu66.top

[J08] 提取年月日与星期
来源：http://nfo.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qhn.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ved.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jcb.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://boo.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rll.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhp.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shf.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nsp.aizwys.cn

[J09] 时区处理
来源：http://pzw.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dwm.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfm.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzr.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ikm.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jwi.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vxs.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vrb.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://anp.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://siy.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gru.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wvb.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jdc.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pqs.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pjl.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ebc.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ozz.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nyi.xingfuxueyuan.xyz

================================================================================
来源：http://qrf.jinqigfzy.top

K. JSON 与序列化
来源：http://sgh.shuidangran.top

================================================================================
来源：http://emu.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ucl.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixu.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mls.sweek.top

JS:   JSON.stringify(obj)
来源：http://gut.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://mce.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wkb.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://klv.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://qqk.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jbe.yj202588.top

[K02] JSON 字符串转对象
来源：http://rfa.aizwys.cn

Py:   json.loads(s)
来源：http://vtu.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aut.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://jph.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://lpp.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jng.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://iew.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://nqv.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lfs.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://gkl.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://peb.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bju.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wdy.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zal.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oui.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ald.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wdk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://voh.yonumen.top

[K04] 读取 JSON 文件
来源：http://cvt.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gbj.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agh.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gjf.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hum.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://irt.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbr.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vbu.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aop.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://kcz.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://yar.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://uzh.wangdashe.top

JS:   structuredClone(obj)
来源：http://mds.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://enk.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://ohh.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fuq.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://klf.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://fdq.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://eti.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://feu.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fcn.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izs.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpg.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://igu.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://iws.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ncj.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vzr.cheryme.top

[K07] 进制转换
来源：http://tdu.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qed.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bhr.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rij.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pcb.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://prw.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://icv.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://why.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sof.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://orw.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://xhb.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pdl.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://mwb.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://pry.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gti.yongpay.top

Go:   encoding/gob
来源：http://xgp.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://qpj.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ubj.fzhhl.top

================================================================================
来源：http://hgb.nanxinkj.top

L. 网络请求
来源：http://caz.wangshuangyany.cn

================================================================================
来源：http://alk.tianlin.xyz

[L01] 发送 GET 请求
来源：http://ogy.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kes.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jkl.hnxiangtu.top

JS:   await fetch(url)
来源：http://rjn.svipenyu.cn

TS:   await fetch(url)
来源：http://dsr.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://muf.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://ico.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://zbg.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aqz.zdqjudy.top

[L02] 发送 POST JSON
来源：http://ysn.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://fhn.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wir.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgx.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://faa.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mjg.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlx.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jsd.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lfk.vehdjk.com

[L03] 设置自定义请求头
来源：http://sry.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eps.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xfm.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hru.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pjq.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tpx.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qve.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jzj.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lrr.ydzc1.top

[L04] 设置超时
来源：http://hzi.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://zvb.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qap.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgv.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsd.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://txo.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mzg.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mih.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nmi.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://kmh.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mwv.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zvw.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://toz.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iwt.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iyf.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://czb.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blg.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zat.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://ppf.zycfv.cn

Py:   resp.json()
来源：http://ean.yuxming.cn

PHP:  json_decode($body, true);
来源：http://qyn.fktsv.cn

JS:   await resp.json()
来源：http://dox.zhongyouzk.top

TS:   await resp.json()
来源：http://cjq.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lgf.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://izs.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://knb.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zoa.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://xvy.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsz.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://arn.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://nvu.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://fcy.kuanghao11.cn

Java: resp.statusCode()
来源：http://dbq.yonumen.top

Go:   resp.StatusCode
来源：http://eij.cashguo.top

Ruby: resp.code.to_i
来源：http://vpk.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://cle.snrcjt.cn

[L08] 并发请求多个地址
来源：http://hdx.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jag.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://sul.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jae.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uqv.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trf.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iby.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dxw.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vxs.yfazqb.com

================================================================================
来源：http://cfe.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ron.nanxinkj.top

================================================================================
来源：http://djr.pycfn.com

[M01] 读取命令行参数
来源：http://wek.tianlin.xyz

Py:   sys.argv[1:]
来源：http://sxi.ydzc1.top

PHP:  $argv;  $argc;
来源：http://hvo.yonumen.top


<!-- 参考信息 -->