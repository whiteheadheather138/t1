代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rnp.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hai.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ves.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mof.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://suk.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdr.ybcxt.top

[I04] 正则替换
来源：http://vdm.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ruq.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zpt.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://sap.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://gwf.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ktl.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uhi.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hzl.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wll.zdqjudy.top

[I05] 按正则拆分
来源：http://tvq.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://txe.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdc.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://rid.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://zwb.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ojs.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wgv.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://rtl.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zxb.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ama.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hrd.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lqo.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujo.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njw.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dqs.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rfj.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pao.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://weu.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://tmo.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yct.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://okw.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hlt.zhaomingkeji.xyz

TS:   /error/gim
来源：http://frx.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rlk.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://paa.316326.xyz

Ruby: s.scan(/error/i)
来源：http://llj.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://urt.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://uwx.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vzc.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vcj.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfi.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxc.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xxp.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vnr.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://som.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://snp.zhaomingkeji.xyz

================================================================================
来源：http://dhc.nanxinkj.top

J. 日期与时间
来源：http://dpd.wangdashe.top

================================================================================
来源：http://ody.tanke756.top

[J01] 获取当前时间
来源：http://hqm.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kil.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kri.ybcxt.top

JS:   new Date();  Date.now()
来源：http://wcg.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://zhp.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://txb.sysykeji.top

Go:   time.Now()
来源：http://tok.dianchejie.cn

Ruby: Time.now
来源：http://cmw.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nza.vehdjk.com

[J02] 格式化输出
来源：http://cne.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iyj.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vzl.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zvt.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://ugl.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tmv.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ggi.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyh.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jly.dashuyun.cn

[J03] 字符串解析为日期
来源：http://gju.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ngp.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bic.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://ght.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://qtc.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://yxt.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pgl.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://amc.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bdv.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://whi.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fek.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vtw.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hyt.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://kct.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eet.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wiq.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vfc.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bvu.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://csv.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://rwn.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sun.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bxk.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uyk.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://hed.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jal.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://ual.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://xvo.epnwcf.com

[J06] 计算两时间之差
来源：http://xzh.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://txl.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://yqe.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ifb.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://thb.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ffz.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://bjd.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://jwa.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://pmd.gogol.net.cn

[J07] 比较两个日期
来源：http://psj.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://yhe.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://orl.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jog.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://puw.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qsm.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jhu.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://nij.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://hlk.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://pex.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pbj.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kbj.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hmh.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ouj.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mib.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvc.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ztm.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rdu.jinqigfzy.top

[J09] 时区处理
来源：http://olv.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cnc.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zmi.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ypi.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nic.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://any.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://evu.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mzw.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fpc.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://uyh.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zor.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dsy.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ivg.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rrf.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gor.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uvy.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gjy.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qyo.tian-w.cn

================================================================================
来源：http://olu.chenlongwang.top

K. JSON 与序列化
来源：http://ewy.yj20258.top

================================================================================
来源：http://xwd.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://ueu.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sry.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://inb.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://zly.birdmap.top

TS:   JSON.stringify(obj)
来源：http://uls.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ymh.daxiang520.top

Go:   json.Marshal(obj)
来源：http://gyt.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://onm.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qfx.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://knf.birdmap.top

Py:   json.loads(s)
来源：http://ttm.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://igi.xuanzx.com

JS:   JSON.parse(s)
来源：http://bng.yueranfly.top

TS:   JSON.parse(s)
来源：http://are.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cjo.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://gpv.fengsongda.top

Ruby: JSON.parse(s)
来源：http://hzv.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ogl.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://rtp.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zwb.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ugo.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://fcp.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://has.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uey.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ctz.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pji.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nrh.guannengcc.top

[K04] 读取 JSON 文件
来源：http://ahz.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fzj.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pdy.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rnn.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nwu.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lwh.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fxb.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://azz.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gat.nanxinkj.top

[K05] 深拷贝对象
来源：http://xyn.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://hpc.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://omx.cqqwz.cn

JS:   structuredClone(obj)
来源：http://rur.wangdashe.top

TS:   structuredClone(obj)
来源：http://alf.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://fwu.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tzb.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uos.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hly.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://gsv.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qna.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nxd.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ebi.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdg.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gqg.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tvt.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cyi.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hjy.jinqigufen.top

[K07] 进制转换
来源：http://owb.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hls.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hbk.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mrx.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dki.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oqe.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zxw.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uok.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gfr.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://yrl.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://rkz.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vyo.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://nub.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://wgb.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mtf.0kj1m.cn

Go:   encoding/gob
来源：http://sjt.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://otn.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rnf.xziqi.cn

================================================================================
来源：http://qoh.316326.xyz

L. 网络请求
来源：http://fsd.fengsongda.top

================================================================================
来源：http://nsb.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://fxk.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ukv.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cdj.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://dxg.hnxiangtu.top

TS:   await fetch(url)
来源：http://zvv.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sez.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://hde.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oan.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eep.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://icw.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://byg.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yyr.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdk.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fpa.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjr.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://udn.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lqw.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qms.hywenlv.cn

[L03] 设置自定义请求头
来源：http://oin.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yhd.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ixt.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uig.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpk.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yuo.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qgw.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eon.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zks.xziqi.cn

[L04] 设置超时
来源：http://moa.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://idg.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgw.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjv.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://avt.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://enq.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rgo.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cik.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sqk.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://yro.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ktl.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sms.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nli.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zhn.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fut.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mqt.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tef.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sci.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://kjq.vqdsnc.cn

Py:   resp.json()
来源：http://vyf.yvedp.cn

PHP:  json_decode($body, true);
来源：http://eyk.ppjwa.cn

JS:   await resp.json()
来源：http://rjs.xylfe.cn

TS:   await resp.json()
来源：http://zyl.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mkb.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bfd.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://nky.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hnk.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://prc.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rlj.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mtw.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://fbm.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://cuv.cashguo.top

Java: resp.statusCode()
来源：http://wus.uphjek.com

Go:   resp.StatusCode
来源：http://fwc.redwolf501.top

Ruby: resp.code.to_i
来源：http://gqp.pycfn.com

C#:   (int)resp.StatusCode
来源：http://fym.tarul.cn

[L08] 并发请求多个地址
来源：http://syk.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dlo.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://pbo.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kqc.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mpn.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wmm.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dab.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qhb.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pww.yangfankeji.com

================================================================================
来源：http://rlg.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://ous.zdbjq.cn

================================================================================
来源：http://szc.zhongyouzk.top

[M01] 读取命令行参数
来源：http://vmh.jyoumei.cn

Py:   sys.argv[1:]
来源：http://fxd.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://wxh.meibo888.top


<!-- 参考信息 -->