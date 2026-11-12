代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://dwm.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://jvs.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xnt.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://dni.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://lgo.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://iet.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ynr.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://bfq.chenlongwang.top

[G10] 访问控制
来源：http://oyg.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://fjp.sxryk.cn

PHP:  public / protected / private
来源：http://bqg.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://fgj.jqgufenzy.top

TS:   public / protected / private
来源：http://kga.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://fjs.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xzd.epnwcf.com

Ruby: public / protected / private
来源：http://zxs.chenlongwang.top

C#:   public / protected / private / internal
来源：http://vba.shzxlz.cn

[G11] getter / setter
来源：http://wzi.meibo888.top

Py:   @property 与 @x.setter
来源：http://vib.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eqk.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://arz.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://plp.yvedp.cn

Java: public String getName() { return name; }
来源：http://fmt.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbj.hywenlv.cn

Ruby: attr_accessor :name
来源：http://ypt.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://xtg.cqqwz.cn

[G12] 对象转字符串
来源：http://azq.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://cng.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fmb.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://zng.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://ztu.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://syj.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://mkk.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://xwg.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://itr.jqgufenzy.top

[G13] 判断对象类型
来源：http://mgn.fengsongda.top

Py:   isinstance(u, User)
来源：http://skw.daxiang520.top

PHP:  $u instanceof User
来源：http://iut.daria6918.cn

JS:   u instanceof User
来源：http://wur.cashguo.top

TS:   u instanceof User
来源：http://cyg.bbcook.cn

Java: u instanceof User
来源：http://jtd.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://arn.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://mdx.yj20258.top

C#:   u is User
来源：http://bwc.haohaochexian.top

[G14] 数据类 / record
来源：http://moy.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ygy.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://byo.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://zua.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://jle.316326.xyz

Java: record User(String name, int age) {}
来源：http://efl.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://edn.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yky.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://vxf.haohaochexian.top

[G15] 枚举
来源：http://ybp.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://srq.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tbg.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dri.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ypo.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://pzz.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jvg.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://byb.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vwc.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://exg.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yue.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://zdu.andypj.xyz

JS:   Object.entries(obj)
来源：http://lkz.jqgfzy.top

TS:   Object.entries(obj)
来源：http://qmc.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://grp.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oxp.hcnkem.com

Ruby: obj.instance_variables
来源：http://xsy.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://cvx.zhixingplan.top

================================================================================
来源：http://bwb.ppjwa.cn

H. 异常与错误处理
来源：http://gxf.ctjpmb.com

================================================================================
来源：http://muv.guannengcc.top

[H01] try / catch 基础
来源：http://iqo.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gjg.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zgi.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fcv.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uyy.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pmg.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pxt.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hzr.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mhg.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://xqf.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://wja.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://srz.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hzz.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vyl.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://umu.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://khi.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dbz.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mmj.birdmap.top

[H03] 主动抛出异常
来源：http://yem.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://web.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://opn.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://iwn.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://fkf.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mez.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tox.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ccz.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://qbo.yuxming.cn

[H04] 自定义异常类型
来源：http://fal.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://nxo.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tip.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ywy.c1oappe.top

TS:   class MyError extends Error {}
来源：http://glv.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://xgr.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dng.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://hvd.pycfn.com

C#:   class MyException : Exception {}
来源：http://xhs.smart0.xyz

[H05] 捕获特定类型
来源：http://bjo.sweek.top

Py:   except ValueError as e:
来源：http://jru.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nnw.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://duz.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://wto.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://hrz.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ygc.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://hty.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uti.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://wph.hesvh.cn

Py:   value = d.get("k") or default
来源：http://kfo.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://mlh.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://mit.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wgv.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ugj.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://yqr.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://mud.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://jrh.yueranfly.top

[H07] 断言
来源：http://yka.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://tai.havefunace.top

PHP:  assert($x > 0);
来源：http://bse.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://pbz.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://ahg.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://htv.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://akv.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://wao.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://frr.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://kcr.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://xzt.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hny.shuidangran.top

JS:   e.message;  e.stack
来源：http://wgv.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qqt.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ung.mhx1999.top

Go:   err.Error()
来源：http://uww.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://cpn.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://ctp.cashguo.top

[H09] 带错误码的异常
来源：http://nqw.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jic.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pwd.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://twx.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zac.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dqt.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rsq.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oft.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pqz.nanxinkj.top

[H10] 资源自动释放
来源：http://ker.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://orx.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lga.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdh.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rhs.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xmp.jqgfzy.top

Go:   defer f.Close()
来源：http://mub.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://clq.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rea.zycfv.cn

================================================================================
来源：http://wjh.pycfn.com

I. 正则表达式
来源：http://ldm.cdnleiting.top

================================================================================
来源：http://hkq.svipenyu.cn

[I01] 判断是否匹配
来源：http://rji.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gey.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://dsm.gzhubu.top

JS:   /\d+/.test(s)
来源：http://ujk.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://ied.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://maw.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tla.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://bfg.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zxd.sjlbkw.cn

[I02] 提取所有匹配
来源：http://swy.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://qfb.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rda.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qqb.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://qdu.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hip.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://azc.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://ndd.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zft.ydjk.org.cn

[I03] 提取捕获分组
来源：http://pft.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://smd.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hvb.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tcz.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://znm.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bve.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iho.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jtt.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mko.sweek.top

[I04] 正则替换
来源：http://xfp.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ess.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jwm.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://vzp.shuidangran.top

TS:   s.replace(/\d+/g, "#")
来源：http://aie.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fdg.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://moh.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://crc.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lry.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://mcc.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ick.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://stn.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://hyb.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://xuo.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://ntz.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://daz.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://hln.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vhn.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qmu.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xps.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rmm.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iix.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwa.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ghe.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mee.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ant.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cls.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://yya.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kwy.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rwh.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dif.fzhhl.top

TS:   /error/gim
来源：http://wqy.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yvd.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pay.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://rlo.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ljz.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://lbu.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rkq.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://opl.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwd.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://grk.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xxp.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yyg.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gyc.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fui.yonumen.top

================================================================================
来源：http://ems.shuidangran.top

J. 日期与时间
来源：http://osw.nwbrower.top

================================================================================
来源：http://hpv.tian-w.cn

[J01] 获取当前时间
来源：http://mel.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bha.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://los.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://osg.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://iie.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qcr.havefunace.top

Go:   time.Now()
来源：http://zec.aizwys.cn

Ruby: Time.now
来源：http://kla.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvh.yangfankeji.com

[J02] 格式化输出
来源：http://ctt.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nwu.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pgn.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oqm.vehdjk.com

TS:   d.toISOString()
来源：http://dky.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lzk.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vgy.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svn.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ctv.smart0.xyz

[J03] 字符串解析为日期
来源：http://uaf.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rwi.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qji.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://icl.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://sfh.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eyc.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhn.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://xly.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gbg.zycfv.cn

[J04] 时间戳与日期互转
来源：http://hiu.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zye.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ltx.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://por.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jfn.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ccv.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jnw.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lhz.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://obz.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://kij.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://xiv.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eec.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ild.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nxy.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://mog.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xpj.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://emd.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://svj.dashuyun.cn

[J06] 计算两时间之差
来源：http://uch.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://alv.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://jad.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mjh.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wsx.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cte.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://kjq.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://gpa.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://xid.0kj1m.cn

[J07] 比较两个日期
来源：http://ule.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://twr.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uuw.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://bst.guowangkeji.top


<!-- 参考信息 -->