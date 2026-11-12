代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fuv.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xqz.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zcy.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vyl.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rio.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oll.yuanzhike.top

[I04] 正则替换
来源：http://hzn.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fyd.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cic.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jef.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://xdv.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mlk.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cwn.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fid.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bia.bjfxy.top

[I05] 按正则拆分
来源：http://aii.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uqy.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yff.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://wss.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://lac.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://wui.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kcx.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://eka.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xsm.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kes.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ysc.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zao.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxa.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rby.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ilg.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eox.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gpl.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dsc.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://qha.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nlv.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eud.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ukf.daria6918.cn

TS:   /error/gim
来源：http://psw.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccj.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pxg.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://vmc.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tlu.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://ofn.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iuw.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rps.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lup.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ror.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fpi.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://our.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mpb.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://amo.jyoumei.cn

================================================================================
来源：http://rjk.yanxiufei.cn

J. 日期与时间
来源：http://roz.tian-w.cn

================================================================================
来源：http://pkh.yangfankeji.com

[J01] 获取当前时间
来源：http://pkm.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://lyj.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://awk.fehbvm.com

JS:   new Date();  Date.now()
来源：http://uhx.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://drm.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://clz.hammf.cn

Go:   time.Now()
来源：http://pmr.gotoacloud.top

Ruby: Time.now
来源：http://tpl.hongshengwenyu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jlb.hfpthk.cn

[J02] 格式化输出
来源：http://qoa.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doh.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bek.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tpq.aizwys.cn

TS:   d.toISOString()
来源：http://hsg.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gkg.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ypl.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://znr.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jcq.gogol.net.cn

[J03] 字符串解析为日期
来源：http://uro.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vmz.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://drw.yj20258.top

JS:   new Date("2024-01-02")
来源：http://zcr.hammf.cn

TS:   new Date("2024-01-02")
来源：http://qne.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qse.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ylp.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://qfp.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fvr.yueranfly.top

[J04] 时间戳与日期互转
来源：http://ybj.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pau.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pjx.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qdb.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ptw.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bbu.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://epi.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wtu.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iri.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://dpk.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://lgk.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qpa.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltf.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvq.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://qfq.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bdl.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://rrm.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://oxg.zhengqikj.top

[J06] 计算两时间之差
来源：http://nbs.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://hxx.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://qod.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fkf.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jsu.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://bep.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://ioi.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://vfi.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://uzj.aizwys.cn

[J07] 比较两个日期
来源：http://fhb.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://keg.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ucj.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://rfq.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lzr.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kij.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ujn.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xum.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://nhs.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://sqo.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pww.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nnf.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yto.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uui.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsr.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xav.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agn.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dto.xziqi.cn

[J09] 时区处理
来源：http://zxy.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ryk.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcb.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzc.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqb.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nkg.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yak.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zzf.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bxb.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://emx.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jiq.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rqm.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mcv.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kkh.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fzx.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jnr.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lqo.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xcm.hnxiangtu.top

================================================================================
来源：http://vnu.pycfn.com

K. JSON 与序列化
来源：http://akf.sufxvd.cn

================================================================================
来源：http://ahq.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://oug.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bad.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yud.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://twt.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://sst.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nqk.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://xtc.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://ofc.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zzp.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://vex.jqgufenzy.top

Py:   json.loads(s)
来源：http://gqe.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxs.yangfankeji.com

JS:   JSON.parse(s)
来源：http://bwe.svipenyu.cn

TS:   JSON.parse(s)
来源：http://jkf.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://asr.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://cjq.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://xfy.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://znl.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://yfl.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ufa.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqq.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://asg.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eej.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vlg.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jvs.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://ksw.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zye.pycfn.com

[K04] 读取 JSON 文件
来源：http://kwp.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jsm.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcp.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bgd.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ybx.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vks.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kpt.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://krg.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dfi.hnxiangtu.top

[K05] 深拷贝对象
来源：http://rmk.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://mhy.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://mqo.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://skm.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://sio.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ryy.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gcl.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qpm.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xnq.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://dhh.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qiw.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zgw.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://icg.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kfg.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ksz.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://eri.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gry.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mqb.feifeiyinyue.top

[K07] 进制转换
来源：http://qsc.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmq.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jgz.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rss.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vdh.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hri.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tuo.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ekt.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drn.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ozf.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://wwv.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vmi.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://eax.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://zwg.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wff.uphjek.com

Go:   encoding/gob
来源：http://mlv.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://stp.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://toz.yuanzhike.top

================================================================================
来源：http://cwo.xziqi.cn

L. 网络请求
来源：http://uja.9152youxi.cn

================================================================================
来源：http://ubj.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://vlg.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://loy.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nym.chenjidiqi.icu

JS:   await fetch(url)
来源：http://dzf.zdbjq.cn

TS:   await fetch(url)
来源：http://ceh.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rvw.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://dho.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ote.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jyi.fengsongda.top

[L02] 发送 POST JSON
来源：http://tlf.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://iiz.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qkg.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sih.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbo.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vix.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ekl.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rsn.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jxd.yangfankeji.com

[L03] 设置自定义请求头
来源：http://dzz.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pqi.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xzt.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgj.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gyr.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lhx.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rtz.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wmq.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cvy.tanke756.top

[L04] 设置超时
来源：http://fsk.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://njo.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uas.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttc.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hno.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wnd.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yum.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://krg.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ktp.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://qta.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://png.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zoc.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gsd.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qil.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://izc.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gkw.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dva.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jff.cheryme.top

[L06] 解析响应为 JSON
来源：http://csa.kuanghao11.cn

Py:   resp.json()
来源：http://zqk.pycfn.com

PHP:  json_decode($body, true);
来源：http://qfp.gotoacloud.top

JS:   await resp.json()
来源：http://hjl.sufxvd.cn

TS:   await resp.json()
来源：http://jfo.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vix.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tpn.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://jri.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://une.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://lkm.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjz.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gdb.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://mmv.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://krs.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://acq.ctjpmb.com

Go:   resp.StatusCode
来源：http://jxs.tian-w.cn

Ruby: resp.code.to_i
来源：http://qrq.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://qwo.yueranfly.top

[L08] 并发请求多个地址
来源：http://xfs.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rqu.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://tvp.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gry.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kzl.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://czw.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qks.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://srr.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://epa.fktsv.cn

================================================================================
来源：http://fvm.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://etw.quarkkingdee.top

================================================================================
来源：http://civ.yanxiufei.cn

[M01] 读取命令行参数
来源：http://ypt.yongpay.top

Py:   sys.argv[1:]
来源：http://esw.tanke756.top

PHP:  $argv;  $argc;
来源：http://jus.guannengcc.top


<!-- 参考信息 -->