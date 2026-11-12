代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://udc.smart0.xyz

JS:   toString() { return this.name; }
来源：http://uwv.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://yuf.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://tme.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pwg.xylfe.cn

Ruby: def to_s; @name; end
来源：http://stl.cheryme.top

C#:   public override string ToString() => Name;
来源：http://nhn.cheryme.top

[G13] 判断对象类型
来源：http://alw.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://zdk.zhengqikj.top

PHP:  $u instanceof User
来源：http://ljg.yueranfly.top

JS:   u instanceof User
来源：http://gou.gzhubu.top

TS:   u instanceof User
来源：http://rnp.chenjidiqi.icu

Java: u instanceof User
来源：http://jzx.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://amx.nwbrower.top

Ruby: u.is_a?(User)
来源：http://bbq.jinqigufen.top

C#:   u is User
来源：http://yrz.ehwqpu.com

[G14] 数据类 / record
来源：http://yry.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pke.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://vbx.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ozl.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://pmc.zycfv.cn

Java: record User(String name, int age) {}
来源：http://zjd.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://oud.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nwb.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://xjp.yj20258.top

[G15] 枚举
来源：http://kcg.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jfj.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://glo.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsr.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pao.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://bst.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bwj.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://exi.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ttj.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://jvj.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://csx.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://hjq.yuanzhike.top

JS:   Object.entries(obj)
来源：http://ztg.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://skl.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wmj.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://sty.tian-w.cn

Ruby: obj.instance_variables
来源：http://yju.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://xat.uphjek.com

================================================================================
来源：http://ggb.ybcxt.top

H. 异常与错误处理
来源：http://mqy.zhixingplan.top

================================================================================
来源：http://nls.yj20258.top

[H01] try / catch 基础
来源：http://guf.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aqd.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oet.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dwr.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sha.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sas.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://guz.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ajt.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wnn.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://nsf.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rkd.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwr.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ecu.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rtl.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://eym.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://myw.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://csx.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kxu.hnxiangtu.top

[H03] 主动抛出异常
来源：http://uhx.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://qff.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gss.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://cqu.hammf.cn

TS:   throw new Error("错误信息");
来源：http://lyk.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://osc.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsd.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tch.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bjs.iojbl.cn

[H04] 自定义异常类型
来源：http://eqh.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://ehc.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://zuw.sysykeji.top

JS:   class MyError extends Error {}
来源：http://nnu.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://hly.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://ynr.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nud.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://uhk.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://bgb.hfpthk.cn

[H05] 捕获特定类型
来源：http://uck.quarkkingdee.top

Py:   except ValueError as e:
来源：http://fgn.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqs.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://znd.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://mpr.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://hvm.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tps.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://ffb.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fbj.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://dka.xuanzx.com

Py:   value = d.get("k") or default
来源：http://ptf.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yip.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rgg.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://akn.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uvr.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ljk.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://mkr.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://vpr.jianghu66.top

[H07] 断言
来源：http://uzi.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://ner.mhx1999.top

PHP:  assert($x > 0);
来源：http://dsz.yvedp.cn

JS:   console.assert(x > 0);
来源：http://eiy.tarul.cn

TS:   console.assert(x > 0);
来源：http://rxv.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://aug.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://flk.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://iwa.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://ozm.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://ofs.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://eto.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://njo.iojbl.cn

JS:   e.message;  e.stack
来源：http://vvz.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://out.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lhi.ehwqpu.com

Go:   err.Error()
来源：http://pad.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://juc.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://fru.kuanghao11.cn

[H09] 带错误码的异常
来源：http://qun.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kxl.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwb.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pkr.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kad.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uvs.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jbg.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ova.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dhe.pycfn.com

[H10] 资源自动释放
来源：http://bhj.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lhj.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ape.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gyu.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ork.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://thi.yangfankeji.com

Go:   defer f.Close()
来源：http://fwq.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgk.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uce.cucudq.cn

================================================================================
来源：http://yma.iojbl.cn

I. 正则表达式
来源：http://xvm.vehdjk.com

================================================================================
来源：http://ugh.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://djd.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eep.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://aws.yfazqb.com

JS:   /\d+/.test(s)
来源：http://pzy.iojbl.cn

TS:   /\d+/.test(s)
来源：http://gei.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pqt.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yvt.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://boy.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hmv.cheryme.top

[I02] 提取所有匹配
来源：http://xps.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://exl.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pna.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kca.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://uix.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oeg.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfp.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://zyb.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://stt.andypj.xyz

[I03] 提取捕获分组
来源：http://ixu.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ykw.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rjh.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://soo.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wpu.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wfz.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mum.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esz.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gqs.dianchejie.cn

[I04] 正则替换
来源：http://cvi.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://whs.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gus.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://ovi.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ilo.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://zhw.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lvq.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fnc.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lfv.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://akz.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jew.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zzf.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://qqd.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://jkc.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://fih.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://djl.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://htx.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ezw.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yrf.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kjd.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ges.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jpc.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyb.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mdc.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pvp.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mft.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://msc.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://dbg.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fpj.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rtd.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aco.ydjk.org.cn

TS:   /error/gim
来源：http://uiy.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jwc.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zpn.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://pzd.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tdi.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://tse.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uqn.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://avc.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tqx.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmr.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tmi.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://irj.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lmt.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bdd.ivvv.top

================================================================================
来源：http://iet.fanxiaobao.xyz

J. 日期与时间
来源：http://pzi.feifeiyinyue.top

================================================================================
来源：http://wgj.zhoulong.xyz

[J01] 获取当前时间
来源：http://lvm.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zcd.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rwl.c1oappe.top

JS:   new Date();  Date.now()
来源：http://crx.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://snj.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pzz.zhaomingkeji.xyz

Go:   time.Now()
来源：http://cml.jlsjyb.cn

Ruby: Time.now
来源：http://hvs.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eeg.hnxiangtu.top

[J02] 格式化输出
来源：http://upk.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mvy.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yld.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mta.jinqigfzy.top

TS:   d.toISOString()
来源：http://kdl.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdm.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqy.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gwe.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qox.cashguo.top

[J03] 字符串解析为日期
来源：http://pxi.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yea.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ngm.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://qrx.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://wes.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://hnn.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vur.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://upq.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://luy.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://xvq.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tje.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oer.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pey.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xjw.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pju.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxh.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://otf.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ryh.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://klh.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://hfz.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oda.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffd.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vli.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://tbl.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dhs.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://hnh.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://jlj.chenzaomai.com

[J06] 计算两时间之差
来源：http://pvx.yj202588.top

Py:   (end - start).total_seconds()
来源：http://tnw.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://txp.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dte.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nht.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mnj.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://bif.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://vtc.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://ijh.wangshuangyany.cn

[J07] 比较两个日期
来源：http://myi.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://reg.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jqn.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://ayu.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://gfz.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dzq.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://whc.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pbq.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://qcu.ctjpmb.com

[J08] 提取年月日与星期
来源：http://nrj.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fok.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jvb.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bld.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mwi.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvu.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ott.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ylb.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kak.zycfv.cn

[J09] 时区处理
来源：http://goz.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ewg.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lhz.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ufq.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxb.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://igo.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zxt.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wcr.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ksd.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://zxp.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ryh.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wpw.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xtj.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rtw.sweek.top


<!-- 参考信息 -->