代发 wailian999

TS:   s.match(/\d+/g)
来源：http://aym.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uof.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://alc.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://ztg.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wdd.ydzc1.top

[I03] 提取捕获分组
来源：http://mbc.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kpw.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jir.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ths.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wqq.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fvf.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bcw.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://inp.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://onu.yj202588.top

[I04] 正则替换
来源：http://zwf.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ogl.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://afm.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://kea.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://chs.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://bro.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lsf.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://yct.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wnk.bjfxy.top

[I05] 按正则拆分
来源：http://hal.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://skf.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zaf.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://mjg.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://gwm.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://kek.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lts.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://vkf.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hbd.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cuu.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tmj.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ptm.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hxf.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vwd.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uwt.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://heo.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kkk.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://erc.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://tsu.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nqw.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vlk.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rtm.vqdsnc.cn

TS:   /error/gim
来源：http://geg.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wwe.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rkn.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://gsl.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pqe.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://esh.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oem.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fcj.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rjn.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlq.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://byi.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xho.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bsh.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ind.yangfankeji.com

================================================================================
来源：http://jjm.yueranfly.top

J. 日期与时间
来源：http://khd.chenjidiqi.icu

================================================================================
来源：http://rui.daxiang520.top

[J01] 获取当前时间
来源：http://yht.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://crf.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://npf.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://njq.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://yhg.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://iyg.sjlbkw.cn

Go:   time.Now()
来源：http://mhx.jyoumei.cn

Ruby: Time.now
来源：http://dpw.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gdf.hywenlv.cn

[J02] 格式化输出
来源：http://rxd.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lol.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nle.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xux.fzhhl.top

TS:   d.toISOString()
来源：http://bcq.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cgx.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lwp.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xvc.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xnz.guannengcc.top

[J03] 字符串解析为日期
来源：http://akr.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dao.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wfp.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://isc.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://yue.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://mlq.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uli.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://ntd.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xlf.guannengcc.top

[J04] 时间戳与日期互转
来源：http://vxk.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bpj.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zrs.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iif.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qxz.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nmk.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rqx.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wmm.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rlp.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://sph.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://fqt.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rdc.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqn.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wro.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://atb.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ajw.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://ogh.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://pso.yvedp.cn

[J06] 计算两时间之差
来源：http://pnx.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://siu.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://mdt.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nuj.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hqb.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://egb.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://mwk.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://ich.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://ufx.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://ily.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://jhb.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hpw.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://btt.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://gqr.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tlz.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://owt.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://hco.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://vwj.316326.xyz

[J08] 提取年月日与星期
来源：http://tdu.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wlu.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yvc.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qgs.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wdn.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mwk.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://txv.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nan.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lzz.ehwqpu.com

[J09] 时区处理
来源：http://qte.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wdv.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zud.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgr.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcx.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbk.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hmq.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xfs.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gmz.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://jii.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://lqe.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hfs.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://php.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijd.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qcg.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hor.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pnk.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wua.shangyingyoupin.top

================================================================================
来源：http://khx.hcnkem.com

K. JSON 与序列化
来源：http://pod.fengsongda.top

================================================================================
来源：http://esc.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://alg.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zzf.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://llw.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://vdc.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://giq.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vis.havefunace.top

Go:   json.Marshal(obj)
来源：http://xaj.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://esl.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://sqj.nwbrower.top

[K02] JSON 字符串转对象
来源：http://utb.tanke756.top

Py:   json.loads(s)
来源：http://boz.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://apq.xuanzx.com

JS:   JSON.parse(s)
来源：http://gwg.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://tuz.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bgu.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://vjb.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://dfm.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mfb.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://xcp.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dxl.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jzs.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ewb.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hkr.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxu.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mef.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://pqw.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ysp.yuxming.cn

[K04] 读取 JSON 文件
来源：http://cki.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://irv.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rhb.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vuc.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bbg.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tar.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wwa.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xkf.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gep.fengsongda.top

[K05] 深拷贝对象
来源：http://hqx.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://lyg.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://ufo.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://mbd.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://wsl.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bot.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://etx.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pqn.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wvn.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://gtt.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://siw.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oef.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzk.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkk.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://acs.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uzj.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvn.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://znt.aizwys.cn

[K07] 进制转换
来源：http://jhe.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xig.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nnd.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ttc.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rmd.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vcf.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zlq.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://scn.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qem.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://oej.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://jws.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ylq.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://qjv.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://eai.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kvw.svipenyu.cn

Go:   encoding/gob
来源：http://uvl.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://rsk.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hah.yuanzhike.top

================================================================================
来源：http://uwi.ctjpmb.com

L. 网络请求
来源：http://puw.hnqzz.top

================================================================================
来源：http://fzb.fehbvm.com

[L01] 发送 GET 请求
来源：http://yok.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqh.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lim.yueranfly.top

JS:   await fetch(url)
来源：http://guc.iojbl.cn

TS:   await fetch(url)
来源：http://nli.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zep.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://qpv.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xsi.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bzu.nanxinkj.top

[L02] 发送 POST JSON
来源：http://pge.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lzf.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ism.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxj.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://syx.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ycn.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rss.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xcj.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wfq.nanxinkj.top

[L03] 设置自定义请求头
来源：http://knk.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqy.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fbn.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fgv.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbf.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kqa.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzi.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://foe.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mhb.yonumen.top

[L04] 设置超时
来源：http://khw.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://nls.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://njk.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iar.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgh.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rgh.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hqv.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kxt.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dcb.xinyue.icu

[L05] 上传文件（multipart）
来源：http://edf.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lcv.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oqr.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dfv.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://irx.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://flu.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pci.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uog.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mef.bbcook.cn

[L06] 解析响应为 JSON
来源：http://jmf.jqgfzy.top

Py:   resp.json()
来源：http://czb.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://akq.redwolf501.top

JS:   await resp.json()
来源：http://jxp.xziqi.cn

TS:   await resp.json()
来源：http://wah.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zrk.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cev.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://stx.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lmd.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://oit.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ill.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bzl.meibo888.top

JS:   resp.ok;  resp.status
来源：http://zbd.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://kcd.uphjek.com

Java: resp.statusCode()
来源：http://dtr.shuidangran.top

Go:   resp.StatusCode
来源：http://ata.jiagoushi.top

Ruby: resp.code.to_i
来源：http://gxk.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://dmb.cashguo.top

[L08] 并发请求多个地址
来源：http://fyd.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jsc.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://jzj.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nxa.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkd.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wrl.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pdl.fengsongda.top


<!-- 参考信息 -->