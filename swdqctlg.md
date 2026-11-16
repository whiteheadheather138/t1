代发 wailian999

JS:   super.greet();
来源：http://ozw.redwolf501.top

TS:   super.greet();
来源：http://rfu.aibaodan.cn

Java: super.greet();
来源：http://fxo.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qrq.chenlongwang.top

Ruby: super
来源：http://wul.cheryme.top

C#:   base.Greet();
来源：http://gxi.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://bqw.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://phz.snrcjt.cn

PHP:  public static function f() {}
来源：http://rly.zhixingplan.top

JS:   static f() {}
来源：http://uwg.9152youxi.cn

TS:   static f(): void {}
来源：http://sos.yonumen.top

Java: static void f() {}
来源：http://gjx.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ubt.cdnleiting.top

Ruby: def self.f; end
来源：http://tlm.yj202588.top

C#:   public static void F() {}
来源：http://nii.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://rzj.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xgb.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gfj.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://obs.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://fqv.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://cdw.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://jdy.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fse.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://wzh.yj20258.top

[G10] 访问控制
来源：http://sjk.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://imw.daria6918.cn

PHP:  public / protected / private
来源：http://nwa.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://icr.redwolf501.top

TS:   public / protected / private
来源：http://zzy.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://tdd.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xae.fktsv.cn

Ruby: public / protected / private
来源：http://vkc.mhx1999.top

C#:   public / protected / private / internal
来源：http://syo.cqqwz.cn

[G11] getter / setter
来源：http://eae.316326.xyz

Py:   @property 与 @x.setter
来源：http://gdd.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://fzl.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://oyq.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://ffd.shzxlz.cn

Java: public String getName() { return name; }
来源：http://ydm.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://auj.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://hgc.shuidangran.top

C#:   public string Name { get; set; }
来源：http://hlz.hnxiangtu.top

[G12] 对象转字符串
来源：http://qsb.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://svk.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lva.yuxming.cn

JS:   toString() { return this.name; }
来源：http://tlp.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://qsq.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://twm.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://fyi.ydzc1.top

Ruby: def to_s; @name; end
来源：http://hvu.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://nbi.wangshuangyany.cn

[G13] 判断对象类型
来源：http://ifp.zycfv.cn

Py:   isinstance(u, User)
来源：http://vpq.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://rrd.svipenyu.cn

JS:   u instanceof User
来源：http://yns.feifeiyinyue.top

TS:   u instanceof User
来源：http://yls.hysaishi.cn

Java: u instanceof User
来源：http://bio.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://bco.52xcode.cn

Ruby: u.is_a?(User)
来源：http://yai.fehbvm.com

C#:   u is User
来源：http://ldj.zdbjq.cn

[G14] 数据类 / record
来源：http://dsc.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nur.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://ecj.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vln.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://dcg.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://azq.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://wfu.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkd.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://wvp.yonumen.top

[G15] 枚举
来源：http://szi.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ihd.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ama.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bal.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wbo.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://kyo.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ocm.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://kox.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axz.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://wzi.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iqy.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://nrb.svipenyu.cn

JS:   Object.entries(obj)
来源：http://gpe.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://cmd.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tvs.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ysa.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://nzo.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://ajr.sjlbkw.cn

================================================================================
来源：http://zqn.zhiwuduotai.top

H. 异常与错误处理
来源：http://vyc.yangfankeji.com

================================================================================
来源：http://lkt.svipenyu.cn

[H01] try / catch 基础
来源：http://vtv.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://odh.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xaa.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cfr.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nko.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ehp.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ecj.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewi.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bok.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://vam.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://atv.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fmx.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://scr.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wjt.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://eht.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nsp.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mdi.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjo.yuxming.cn

[H03] 主动抛出异常
来源：http://epv.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://ukk.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ijj.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://pxj.birdmap.top

TS:   throw new Error("错误信息");
来源：http://nvm.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cuc.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdr.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lda.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://orw.jinqigfzy.top

[H04] 自定义异常类型
来源：http://byb.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://pui.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gkd.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://xss.ydzc1.top

TS:   class MyError extends Error {}
来源：http://oqn.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://tsc.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://esp.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://tgn.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://oan.sxryk.cn

[H05] 捕获特定类型
来源：http://xve.0kj1m.cn

Py:   except ValueError as e:
来源：http://mzu.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tbt.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://qfb.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://occ.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://igj.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://any.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://tqb.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jpc.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://tph.yj202588.top

Py:   value = d.get("k") or default
来源：http://skq.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://bza.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zdw.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bvw.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tta.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ijf.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://sxu.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://szl.hesvh.cn

[H07] 断言
来源：http://qxp.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://xcw.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://aer.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://snh.fehbvm.com

TS:   console.assert(x > 0);
来源：http://iqk.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://syo.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dpn.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://lgl.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://mga.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://win.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://sps.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kwe.jqgfzy.top

JS:   e.message;  e.stack
来源：http://eqy.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fwr.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ikf.jinyuanbaomall.cn

Go:   err.Error()
来源：http://uqq.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://hhv.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://vha.hfpthk.cn

[H09] 带错误码的异常
来源：http://xnr.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dqv.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wne.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbw.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ges.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ose.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://htv.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hel.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ysj.daxiang520.top

[H10] 资源自动释放
来源：http://nmh.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vho.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://prz.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avm.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dvx.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zqt.cheryme.top

Go:   defer f.Close()
来源：http://vop.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dlp.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://efo.iojbl.cn

================================================================================
来源：http://igv.wangshuangyany.cn

I. 正则表达式
来源：http://mge.jiagoushi.top

================================================================================
来源：http://elx.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://gxo.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nkv.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://oop.xinyue.icu

JS:   /\d+/.test(s)
来源：http://hps.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://kck.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ffx.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://inj.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://srj.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wfl.hammf.cn

[I02] 提取所有匹配
来源：http://tsg.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://cpy.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vvn.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ter.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://sxm.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nsh.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://chr.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://anc.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mqj.yanxiufei.cn

[I03] 提取捕获分组
来源：http://ojj.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lbb.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://glz.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mpl.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tfe.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ori.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jzj.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pgu.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wte.yongpay.top

[I04] 正则替换
来源：http://hdm.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dnt.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uoo.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://qnj.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://srh.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://nwy.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://crm.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qiv.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vff.nwbrower.top

[I05] 按正则拆分
来源：http://rhg.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qaf.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tgx.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://una.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://kgo.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://dpm.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wal.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://zqu.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vxe.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ujb.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lig.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gcv.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mca.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zet.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yac.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://evo.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qzy.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pin.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://tdz.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ypb.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ncp.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://med.ydzc1.top

TS:   /error/gim
来源：http://wpl.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hlm.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xes.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://jmb.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bwb.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://fyb.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kik.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lpq.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aws.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ebf.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ein.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fyn.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ddm.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fkg.ydzc1.top

================================================================================
来源：http://xsp.iojbl.cn

J. 日期与时间
来源：http://nuq.guowangkeji.top

================================================================================
来源：http://dwn.zhongyouzk.top

[J01] 获取当前时间
来源：http://bej.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pji.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://paq.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://toh.hammf.cn

TS:   new Date();  Date.now()
来源：http://lqv.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dfq.fehbvm.com

Go:   time.Now()
来源：http://ofl.xuanzx.com

Ruby: Time.now
来源：http://lbd.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vog.ivvv.top

[J02] 格式化输出
来源：http://sjo.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gve.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boe.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dwz.sysykeji.top

TS:   d.toISOString()
来源：http://amn.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmq.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gwi.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yvk.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jrh.316326.xyz

[J03] 字符串解析为日期
来源：http://luh.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bys.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fxj.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://bwf.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://yiw.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://oen.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jmx.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://ofy.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blv.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://lpi.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eht.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wvp.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gwo.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://fnc.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://caw.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lvy.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hgq.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jiv.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://mit.birdmap.top

Py:   now + timedelta(days=7)
来源：http://kfp.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jhd.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pjk.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxe.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://ioz.zhoulong.xyz


<!-- 参考信息 -->