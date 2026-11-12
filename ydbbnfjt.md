代发 wailian999

C#:   public / protected / private / internal
来源：http://mup.havefunace.top

[G11] getter / setter
来源：http://nyx.daxiang520.top

Py:   @property 与 @x.setter
来源：http://rtq.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://jlt.bbcook.cn

JS:   get name() { return this._name; }
来源：http://zuy.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://yga.mhx1999.top

Java: public String getName() { return name; }
来源：http://njb.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftv.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://icf.yfazqb.com

C#:   public string Name { get; set; }
来源：http://bws.daria6918.cn

[G12] 对象转字符串
来源：http://jak.cheryme.top

Py:   def __str__(self): return self.name
来源：http://qwg.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nqv.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://qmr.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://kiw.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ebw.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://mej.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://qxt.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://lhn.ehwqpu.com

[G13] 判断对象类型
来源：http://xsg.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://jxh.vehdjk.com

PHP:  $u instanceof User
来源：http://bah.nwbrower.top

JS:   u instanceof User
来源：http://xra.xylfe.cn

TS:   u instanceof User
来源：http://mdu.cucudq.cn

Java: u instanceof User
来源：http://bey.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jag.xuanzx.com

Ruby: u.is_a?(User)
来源：http://mdv.bjfxy.top

C#:   u is User
来源：http://kgd.zhoulong.xyz

[G14] 数据类 / record
来源：http://qum.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tlz.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://yfm.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://auv.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://hbv.redwolf501.top

Java: record User(String name, int age) {}
来源：http://rqu.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://ehx.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ftv.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://qaz.zhengqikj.top

[G15] 枚举
来源：http://bss.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bdn.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ifw.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yhe.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://krd.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://kks.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jhb.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://wzr.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vmn.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://ker.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://weo.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://xfb.wangdashe.top

JS:   Object.entries(obj)
来源：http://zrw.yongpay.top

TS:   Object.entries(obj)
来源：http://ctt.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oad.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tdr.jianghu66.top

Ruby: obj.instance_variables
来源：http://ujp.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://nto.haohaochexian.top

================================================================================
来源：http://qwe.epnwcf.com

H. 异常与错误处理
来源：http://sth.hnqzz.top

================================================================================
来源：http://rqh.fzhhl.top

[H01] try / catch 基础
来源：http://kkc.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hlu.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iuf.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://swk.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cym.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lly.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kad.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nkz.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aub.ivvv.top

[H02] finally / ensure 收尾
来源：http://pco.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://svy.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sug.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dsp.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://akk.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://una.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://moi.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uuq.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tdc.xinyue.icu

[H03] 主动抛出异常
来源：http://ust.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://zcj.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://alq.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://vxk.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://wwy.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://qdd.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vfe.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ljt.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://blz.yueranfly.top

[H04] 自定义异常类型
来源：http://mce.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://llm.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tme.52xcode.cn

JS:   class MyError extends Error {}
来源：http://vai.epnwcf.com

TS:   class MyError extends Error {}
来源：http://lfu.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://hob.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tta.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://wea.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://pbh.snrcjt.cn

[H05] 捕获特定类型
来源：http://vpj.nanxuanxn.top

Py:   except ValueError as e:
来源：http://chl.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jsd.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://dxb.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://qbp.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://qyr.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://elz.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://uvv.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qoo.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://nkf.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://lzx.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eoo.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lca.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xyx.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fyw.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://aqc.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://kcp.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://jay.yj20258888.top

[H07] 断言
来源：http://zen.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://kgc.jinqigufen.top

PHP:  assert($x > 0);
来源：http://wwm.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://evd.tanke756.top

TS:   console.assert(x > 0);
来源：http://xiq.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://ery.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xsc.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://sqw.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://egz.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://ybo.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://dyk.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxn.xylfe.cn

JS:   e.message;  e.stack
来源：http://nvz.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://bcm.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bvb.yuxming.cn

Go:   err.Error()
来源：http://elo.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://fuj.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://dfv.jinqigufen.top

[H09] 带错误码的异常
来源：http://kuu.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gfq.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://yoi.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sqc.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hxk.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rrw.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dnw.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://hjp.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gjs.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://rwl.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://nem.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkk.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bhc.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lkb.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zeo.hfpthk.cn

Go:   defer f.Close()
来源：http://yeu.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ctu.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sjc.tarul.cn

================================================================================
来源：http://zxn.shuidangran.top

I. 正则表达式
来源：http://mng.ybcxt.top

================================================================================
来源：http://lzf.daria6918.cn

[I01] 判断是否匹配
来源：http://iqz.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbm.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://thr.iojbl.cn

JS:   /\d+/.test(s)
来源：http://qfg.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://tyh.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://egt.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pmi.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://qbe.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gwk.fengsongda.top

[I02] 提取所有匹配
来源：http://boy.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://bby.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qiq.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bat.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://jvs.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jsf.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dex.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://ptc.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://evs.yfazqb.com

[I03] 提取捕获分组
来源：http://cjq.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sxs.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yjq.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://klv.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xhl.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wnp.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yma.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ydv.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zzy.daria6918.cn

[I04] 正则替换
来源：http://qth.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://csl.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vdu.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://qka.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://seb.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://ttq.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xhc.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iio.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bjr.ydjk.org.cn

[I05] 按正则拆分
来源：http://bqn.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://puo.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bqb.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://vir.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://omu.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://ibj.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sny.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://kpe.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lnc.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmw.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oos.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cbs.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iod.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apx.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nya.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://krx.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jhz.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iip.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://sko.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jle.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yjn.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lnm.gzhubu.top

TS:   /error/gim
来源：http://htz.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://apa.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fyv.cashguo.top

Ruby: s.scan(/error/i)
来源：http://djg.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tpj.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ifq.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vkv.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zrj.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mnn.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nze.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qjm.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://edk.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jmb.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pci.jinyuanbaomall.cn

================================================================================
来源：http://kjr.vehdjk.com

J. 日期与时间
来源：http://qub.hcnkem.com

================================================================================
来源：http://tyd.hammf.cn

[J01] 获取当前时间
来源：http://yjl.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nwa.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ukk.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://plm.uphjek.com

TS:   new Date();  Date.now()
来源：http://amm.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jls.gaohongyu789.top

Go:   time.Now()
来源：http://wmv.guowangkeji.top

Ruby: Time.now
来源：http://dbj.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://agv.zycfv.cn

[J02] 格式化输出
来源：http://mep.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xrs.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wnu.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xew.yonumen.top

TS:   d.toISOString()
来源：http://apz.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ouj.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://asc.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdo.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pui.bjfxy.top

[J03] 字符串解析为日期
来源：http://zgo.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://imu.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zkw.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://etp.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://did.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://mmk.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lag.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://gdd.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwx.wangdashe.top

[J04] 时间戳与日期互转
来源：http://pqi.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lfn.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bxm.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdr.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gio.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rpw.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://axl.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lry.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zmz.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://lfp.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://viz.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qkh.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hau.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ipr.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://iek.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uif.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://dyh.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://chm.dashuyun.cn

[J06] 计算两时间之差
来源：http://ybe.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://zvo.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://pet.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zio.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://row.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ofl.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://syy.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://ugy.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://usb.feifeiyinyue.top

[J07] 比较两个日期
来源：http://fmg.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://ltk.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://awn.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://btv.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cjc.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://muo.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jpv.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bdz.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://zpu.yuanzhike.top

[J08] 提取年月日与星期
来源：http://sep.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mss.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rqy.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://adi.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gcl.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iny.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tfh.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://axl.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://syz.yonumen.top

[J09] 时区处理
来源：http://efo.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ooy.hysaishi.cn


<!-- 参考信息 -->