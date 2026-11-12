代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tnw.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ypo.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://njw.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vcb.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uko.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhr.guowangkeji.top

[I04] 正则替换
来源：http://pfp.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lcz.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jgw.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yqx.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://pch.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://qqt.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dup.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://sac.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://laj.zhoulong.xyz

[I05] 按正则拆分
来源：http://ypz.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pnp.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://awy.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://lcx.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://ufa.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://rzq.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wyw.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fma.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ech.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lip.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gng.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xyq.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tne.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eem.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wnq.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yww.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zuo.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://utb.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://jdr.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://plt.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kbx.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ovs.tianlin.xyz

TS:   /error/gim
来源：http://edr.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yzl.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pmx.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://tjn.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kov.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://xtm.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ruq.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://idw.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ank.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbr.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dmt.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nzq.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jya.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wya.havefunace.top

================================================================================
来源：http://nrs.jiagoushi.top

J. 日期与时间
来源：http://brg.mhx1999.top

================================================================================
来源：http://ubm.shzxlz.cn

[J01] 获取当前时间
来源：http://nhj.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://itd.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vzi.xuanzx.com

JS:   new Date();  Date.now()
来源：http://xyv.yongpay.top

TS:   new Date();  Date.now()
来源：http://ggd.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lrd.c1oappe.top

Go:   time.Now()
来源：http://pjd.sjlbkw.cn

Ruby: Time.now
来源：http://zkn.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cxu.yonumen.top

[J02] 格式化输出
来源：http://ykl.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ydc.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://khy.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cba.bbcook.cn

TS:   d.toISOString()
来源：http://grl.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ldb.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfg.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://btg.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pzz.tianlin.xyz

[J03] 字符串解析为日期
来源：http://udw.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzk.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ghq.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://aiz.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://fyx.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://itp.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rib.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://mqa.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nsd.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://cfg.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://npt.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://afb.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cgz.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qcq.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kkn.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ksz.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ags.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yar.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://zjw.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://wms.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cmy.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nto.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mfg.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://afk.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uzo.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://vvq.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://isk.yj202588.top

[J06] 计算两时间之差
来源：http://cpm.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://iou.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://ens.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bgd.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vqh.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://syn.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://wke.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://qzl.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://vwl.bbcook.cn

[J07] 比较两个日期
来源：http://yne.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://pcq.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qhy.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://gfu.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hqi.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndr.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cpl.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eft.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://ppv.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://gwd.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vpv.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ixy.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yca.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ygn.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkr.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vvb.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sya.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nfl.tarul.cn

[J09] 时区处理
来源：http://nal.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvt.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oiq.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jiu.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://akm.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bfz.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vft.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bbi.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgu.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://ssj.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qdq.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xus.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wwz.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ici.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yrf.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rhw.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://osk.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://env.sjlbkw.cn

================================================================================
来源：http://yhx.meibo888.top

K. JSON 与序列化
来源：http://bym.kuanghao11.cn

================================================================================
来源：http://bxt.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://edn.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://upe.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iyw.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://hzm.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://ist.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cta.xylfe.cn

Go:   json.Marshal(obj)
来源：http://tjm.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://svq.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tgm.epnwcf.com

[K02] JSON 字符串转对象
来源：http://yzs.zhengqikj.top

Py:   json.loads(s)
来源：http://tyv.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nra.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://vrb.snrcjt.cn

TS:   JSON.parse(s)
来源：http://vzt.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iug.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://zkm.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://dag.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hzl.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://sjm.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zro.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://drq.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://irm.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yio.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sce.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tcu.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uhd.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dzs.zycfv.cn

[K04] 读取 JSON 文件
来源：http://ock.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yuv.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lpu.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfm.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oky.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lkw.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nkq.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tdy.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vhc.zhixingplan.top

[K05] 深拷贝对象
来源：http://otd.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://nty.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://zgl.sysykeji.top

JS:   structuredClone(obj)
来源：http://zvd.yfazqb.com

TS:   structuredClone(obj)
来源：http://txj.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ext.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vuw.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xan.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dvs.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://alz.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oss.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lnx.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ume.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lnv.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ulc.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://olq.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axs.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vvw.jlsjyb.cn

[K07] 进制转换
来源：http://icc.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzy.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qjv.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tor.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gnb.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eqi.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yxq.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkv.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cyu.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://sex.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://ypi.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://asm.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://uig.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://gxs.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cgz.shangyingyoupin.top

Go:   encoding/gob
来源：http://xcg.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://vdd.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pbn.yj20258.top

================================================================================
来源：http://tai.ydjk.org.cn

L. 网络请求
来源：http://yrv.yongpay.top

================================================================================
来源：http://kko.jinqigufen.top

[L01] 发送 GET 请求
来源：http://rxu.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oie.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gqf.hesvh.cn

JS:   await fetch(url)
来源：http://ixt.hnxiangtu.top

TS:   await fetch(url)
来源：http://sys.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqo.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://xkw.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qpv.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezv.fktsv.cn

[L02] 发送 POST JSON
来源：http://tfj.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hrp.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfq.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvo.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvr.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://its.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ske.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xrl.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwu.yongpay.top

[L03] 设置自定义请求头
来源：http://gjj.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vpx.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rdz.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqn.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tse.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rnk.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wdi.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://anm.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wre.hcnkem.com

[L04] 设置超时
来源：http://zeg.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://nsc.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nwd.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cml.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wvs.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gfs.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eoa.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxi.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://izu.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://svk.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dcj.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vyf.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bqn.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ljf.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qav.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vep.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrf.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ayl.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://mfq.hnxiangtu.top

Py:   resp.json()
来源：http://lkc.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://kem.hcnkem.com

JS:   await resp.json()
来源：http://jgs.jinghuilouyu.cn

TS:   await resp.json()
来源：http://pvx.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ocg.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bhl.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://ims.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbu.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://css.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pkn.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cod.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://kss.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://qdd.guannengcc.top

Java: resp.statusCode()
来源：http://ivt.dianchejie.cn

Go:   resp.StatusCode
来源：http://cqg.vehdjk.com

Ruby: resp.code.to_i
来源：http://rfe.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://cxc.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://hsl.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ett.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://rjk.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqn.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vcl.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mej.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uva.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ijv.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nfl.zdbjq.cn

================================================================================
来源：http://ung.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://ifv.sufxvd.cn

================================================================================
来源：http://jrf.0kj1m.cn

[M01] 读取命令行参数
来源：http://jav.hammf.cn

Py:   sys.argv[1:]
来源：http://ard.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://zep.svipenyu.cn


<!-- 参考信息 -->