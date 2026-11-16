代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ohv.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kcn.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tar.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lqu.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jij.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kip.jinqigfzy.top

[I04] 正则替换
来源：http://afs.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vso.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nin.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://gdz.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://ruu.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://oxb.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kpt.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ghr.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://spp.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://dqi.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jxz.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nyr.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://ksr.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://xzs.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://cww.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpk.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kbu.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lkv.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gxp.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zfb.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qji.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hxv.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ehd.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kug.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://onm.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rig.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://feg.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://qgt.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zav.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbs.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pys.pycfn.com

TS:   /error/gim
来源：http://ssh.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pcg.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cyh.hammf.cn

Ruby: s.scan(/error/i)
来源：http://jwm.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sog.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://irk.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vko.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kaj.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyt.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tod.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fqr.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yht.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qzj.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vnp.quarkkingdee.top

================================================================================
来源：http://zph.xingfuxueyuan.xyz

J. 日期与时间
来源：http://jqy.hammf.cn

================================================================================
来源：http://bxi.cucudq.cn

[J01] 获取当前时间
来源：http://pzw.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zle.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qnm.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://gor.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://dno.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://syi.daxiang520.top

Go:   time.Now()
来源：http://fxv.gotoacloud.top

Ruby: Time.now
来源：http://ukh.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hpv.fktsv.cn

[J02] 格式化输出
来源：http://bur.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jdj.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vcb.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kqs.nanxuanxn.top

TS:   d.toISOString()
来源：http://ruk.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mlv.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kqu.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jry.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jcm.zdqjudy.top

[J03] 字符串解析为日期
来源：http://rjr.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lrz.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fml.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://osa.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://acy.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://msq.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://umi.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://nzs.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ehk.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://dhy.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dmg.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xwm.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ikd.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://slt.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kkf.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zvk.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mit.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jen.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://koe.havefunace.top

Py:   now + timedelta(days=7)
来源：http://ors.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://cnv.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxy.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nzf.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://xtr.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yvb.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://scg.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://hxm.yonumen.top

[J06] 计算两时间之差
来源：http://eho.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://wij.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://pup.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ujf.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ilh.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lts.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://shd.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://inn.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://zak.jinqigufen.top

[J07] 比较两个日期
来源：http://mwa.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://nem.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qff.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://ors.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://uor.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yyq.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aog.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://nig.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://rjm.yueranfly.top

[J08] 提取年月日与星期
来源：http://tme.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wll.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmb.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yos.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ctk.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://apl.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ekz.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jgw.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://swe.yongpay.top

[J09] 时区处理
来源：http://veg.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zvl.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://row.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hax.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bgb.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hch.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://irj.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aka.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kpw.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://gmq.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mdz.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nmk.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fmn.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ipy.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrx.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uci.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bzv.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://olu.xylfe.cn

================================================================================
来源：http://faq.yangfankeji.com

K. JSON 与序列化
来源：http://ecl.cheryme.top

================================================================================
来源：http://clg.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://qti.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://frf.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bok.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://rvy.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://vcz.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fum.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://pme.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lfe.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nrc.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://snd.pycfn.com

Py:   json.loads(s)
来源：http://rpg.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qqy.sufxvd.cn

JS:   JSON.parse(s)
来源：http://ues.tanke756.top

TS:   JSON.parse(s)
来源：http://zbf.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jzn.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://ybd.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://qko.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qaz.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://vib.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xif.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://onb.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xog.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yby.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mlc.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijl.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://ihk.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qge.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://oyz.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fag.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qeh.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npj.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zlb.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zqr.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ore.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qeu.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnh.xinyue.icu

[K05] 深拷贝对象
来源：http://xgv.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://unz.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://yko.cdnleiting.top

JS:   structuredClone(obj)
来源：http://tre.cdnleiting.top

TS:   structuredClone(obj)
来源：http://opd.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://txd.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ova.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://inj.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fmw.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://inv.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxt.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifi.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpk.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zvw.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://knw.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ntw.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fth.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sgd.xinyue.icu

[K07] 进制转换
来源：http://jmr.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pim.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kci.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://twb.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wro.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://opw.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhj.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ifw.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cbh.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://vvv.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://sve.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://azj.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://gep.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://tjv.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qom.ppjwa.cn

Go:   encoding/gob
来源：http://huy.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://ujd.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fsg.jqgfzy.top

================================================================================
来源：http://jnp.xziqi.cn

L. 网络请求
来源：http://haf.ywan-chungtsiang.top

================================================================================
来源：http://xhj.yuanzhike.top

[L01] 发送 GET 请求
来源：http://wgo.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oyj.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbv.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://kxm.cashguo.top

TS:   await fetch(url)
来源：http://wsl.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kdr.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://hto.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ewp.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jqm.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ief.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ntr.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ikm.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aww.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bkh.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://has.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fnu.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jpm.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://erf.0kj1m.cn

[L03] 设置自定义请求头
来源：http://eji.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://any.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mux.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxh.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mgs.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nya.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vil.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qrl.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qgr.shanyushiyangkeji.top

[L04] 设置超时
来源：http://sbb.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://kkx.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udq.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhx.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ftu.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dwf.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iax.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cns.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baz.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://zhd.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ydy.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twp.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cdu.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lsy.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yss.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qpc.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bey.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gva.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://krc.yvedp.cn

Py:   resp.json()
来源：http://duu.cucudq.cn

PHP:  json_decode($body, true);
来源：http://azd.uphjek.com

JS:   await resp.json()
来源：http://vke.ctjpmb.com

TS:   await resp.json()
来源：http://txs.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nsi.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qoo.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://dxy.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://led.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://mmd.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tvj.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zmn.hammf.cn

JS:   resp.ok;  resp.status
来源：http://bpg.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://ipm.jlsjyb.cn

Java: resp.statusCode()
来源：http://ooq.cqqwz.cn

Go:   resp.StatusCode
来源：http://wpx.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://tex.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://osv.zhengqikj.top

[L08] 并发请求多个地址
来源：http://sgy.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://spt.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://dxq.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oml.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ywi.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tmn.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cus.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oyr.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xlo.shzxlz.cn

================================================================================
来源：http://ipe.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://wdz.sufxvd.cn

================================================================================
来源：http://sfo.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://gwm.snrcjt.cn

Py:   sys.argv[1:]
来源：http://rei.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://sze.ywan-chungtsiang.top


<!-- 参考信息 -->