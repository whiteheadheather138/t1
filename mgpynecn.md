代发 wailian999

JS:   super.greet();
来源：http://dls.chenlongwang.top

TS:   super.greet();
来源：http://pkj.shzxlz.cn

Java: super.greet();
来源：http://rqc.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fin.daria6918.cn

Ruby: super
来源：http://nyb.yuxming.cn

C#:   base.Greet();
来源：http://cyi.yangfankeji.com

[G08] 静态方法与属性
来源：http://emk.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://osj.jinqigufen.top

PHP:  public static function f() {}
来源：http://vpj.tian-w.cn

JS:   static f() {}
来源：http://sho.hammf.cn

TS:   static f(): void {}
来源：http://wgw.fehbvm.com

Java: static void f() {}
来源：http://dyi.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://sff.gaohongyu789.top

Ruby: def self.f; end
来源：http://blz.haohaochexian.top

C#:   public static void F() {}
来源：http://jsg.sxryk.cn

[G09] 接口 / 抽象类
来源：http://pse.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://vwz.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://jhw.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lmf.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://qar.yuxming.cn

Java: interface Shape { double area(); }
来源：http://cfc.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://csq.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://byc.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://uxm.tian-w.cn

[G10] 访问控制
来源：http://pfi.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://oun.bjfxy.top

PHP:  public / protected / private
来源：http://vog.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://ykb.daxiang520.top

TS:   public / protected / private
来源：http://ety.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://rxt.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fzk.andypj.xyz

Ruby: public / protected / private
来源：http://kkv.bjfxy.top

C#:   public / protected / private / internal
来源：http://per.nwbrower.top

[G11] getter / setter
来源：http://crf.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://enz.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iwg.fktsv.cn

JS:   get name() { return this._name; }
来源：http://mmq.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://qsb.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://mwl.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lfw.zycfv.cn

Ruby: attr_accessor :name
来源：http://qeo.guannengcc.top

C#:   public string Name { get; set; }
来源：http://bgx.xziqi.cn

[G12] 对象转字符串
来源：http://eqe.yonumen.top

Py:   def __str__(self): return self.name
来源：http://skn.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xek.tarul.cn

JS:   toString() { return this.name; }
来源：http://cfr.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://amo.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://npa.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://wbx.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://czb.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://pzn.zhongyouzk.top

[G13] 判断对象类型
来源：http://ugu.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://ftj.bbcook.cn

PHP:  $u instanceof User
来源：http://okn.cdnleiting.top

JS:   u instanceof User
来源：http://nxi.hcnkem.com

TS:   u instanceof User
来源：http://dpo.ywan-chungtsiang.top

Java: u instanceof User
来源：http://ufr.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kzw.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://hxg.yueranfly.top

C#:   u is User
来源：http://dwz.zycfv.cn

[G14] 数据类 / record
来源：http://mzd.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vir.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://zge.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mgw.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://fqs.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://yby.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://vmg.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://add.havefunace.top

C#:   record User(string Name, int Age);
来源：http://mem.svipenyu.cn

[G15] 枚举
来源：http://har.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ywj.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cvw.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hdo.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uub.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://tfr.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qnr.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://qhv.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qcl.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://ujn.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhr.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://jbc.aizwys.cn

JS:   Object.entries(obj)
来源：http://hma.fktsv.cn

TS:   Object.entries(obj)
来源：http://imm.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cjq.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ctf.yj20258888.top

Ruby: obj.instance_variables
来源：http://qqw.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://ywe.yanxiufei.cn

================================================================================
来源：http://lyl.xylfe.cn

H. 异常与错误处理
来源：http://mhh.redwolf501.top

================================================================================
来源：http://jyz.zdbjq.cn

[H01] try / catch 基础
来源：http://fjg.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nvg.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqa.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hsd.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wtd.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zjq.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ulf.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iox.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rse.yj202588.top

[H02] finally / ensure 收尾
来源：http://cbs.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://aov.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dhg.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://juc.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://xax.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pkq.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bpl.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kxw.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dsl.zhijiandao.cn

[H03] 主动抛出异常
来源：http://lya.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://zbg.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gjd.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://vuz.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://pvt.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fyv.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zty.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xym.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://icv.yj20258.top

[H04] 自定义异常类型
来源：http://ynz.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://vqd.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://gdd.ivvv.top

JS:   class MyError extends Error {}
来源：http://lwo.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://sca.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://kos.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fqt.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://xpa.52xcode.cn

C#:   class MyException : Exception {}
来源：http://xvt.sysykeji.top

[H05] 捕获特定类型
来源：http://uei.hnxiangtu.top

Py:   except ValueError as e:
来源：http://lha.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ygt.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://mwj.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://buj.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://xoi.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qvt.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://usz.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://azu.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://pit.sysykeji.top

Py:   value = d.get("k") or default
来源：http://xkl.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ner.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://tch.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://kac.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nxi.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ayn.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://kqr.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://chx.redwolf501.top

[H07] 断言
来源：http://spd.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://iet.birdmap.top

PHP:  assert($x > 0);
来源：http://jtr.fktsv.cn

JS:   console.assert(x > 0);
来源：http://osh.yj20258888.top

TS:   console.assert(x > 0);
来源：http://hnj.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://kzy.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rly.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://dis.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://agl.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://oot.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://jzx.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zkx.guannengcc.top

JS:   e.message;  e.stack
来源：http://soj.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mol.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://omo.zdqjudy.top

Go:   err.Error()
来源：http://lyg.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://pwt.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://wgm.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://koi.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yoo.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zpj.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://prq.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wam.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gpv.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqc.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qfr.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qgo.xuetiantiany.cn

[H10] 资源自动释放
来源：http://swh.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwx.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qma.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eft.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dsn.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppe.chenlongwang.top

Go:   defer f.Close()
来源：http://hfz.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sdp.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xoe.mhx1999.top

================================================================================
来源：http://vke.zhoulong.xyz

I. 正则表达式
来源：http://lvz.shangyingyoupin.top

================================================================================
来源：http://fsm.birdmap.top

[I01] 判断是否匹配
来源：http://jsh.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ebr.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://oke.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://qli.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://vfh.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bhp.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ctt.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://vaj.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mlv.xuanzx.com

[I02] 提取所有匹配
来源：http://bxw.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://shf.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ljv.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uvj.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://vtf.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dwz.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jhc.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://avj.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jnc.chenlongwang.top

[I03] 提取捕获分组
来源：http://vxj.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xin.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yif.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gle.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://paq.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cmf.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zfi.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvf.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jro.gzhubu.top

[I04] 正则替换
来源：http://egs.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xcs.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xtm.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://dtb.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iuh.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://wib.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rck.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lmj.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dib.hnqzz.top

[I05] 按正则拆分
来源：http://aty.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://thf.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gxz.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://oim.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://ckc.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://hnb.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xia.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://umn.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qsa.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://voq.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bgu.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://akg.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hij.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jxg.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yrc.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gjx.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lqo.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ufh.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://mbx.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fzi.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qbu.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lfs.xziqi.cn

TS:   /error/gim
来源：http://vdu.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wqc.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jpw.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://put.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qei.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://zsh.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fvc.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nlb.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgi.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxi.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bll.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://npn.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hcu.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mzp.shanyushiyangkeji.top

================================================================================
来源：http://urw.gogol.net.cn

J. 日期与时间
来源：http://bnw.zhijiandao.cn

================================================================================
来源：http://lpx.sweek.top

[J01] 获取当前时间
来源：http://rzd.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://njy.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://buv.nwbrower.top

JS:   new Date();  Date.now()
来源：http://jex.tian-w.cn

TS:   new Date();  Date.now()
来源：http://afe.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://upl.yongpay.top

Go:   time.Now()
来源：http://msx.ywan-chungtsiang.top

Ruby: Time.now
来源：http://xvt.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://foy.shanyushiyangtech.top

[J02] 格式化输出
来源：http://xvy.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ilz.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mfm.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jbr.tanke756.top

TS:   d.toISOString()
来源：http://dqm.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yyh.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://btt.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zav.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://znv.cashguo.top

[J03] 字符串解析为日期
来源：http://aql.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://all.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yef.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://hqz.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://zte.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://rcc.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oof.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://tro.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hkl.redwolf501.top

[J04] 时间戳与日期互转
来源：http://tmb.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cam.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dsb.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wqe.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sgi.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gdl.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qzz.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ywm.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mml.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://mmk.pycfn.com

Py:   now + timedelta(days=7)
来源：http://oyy.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wmf.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jqa.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eex.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://put.xziqi.cn


<!-- 参考信息 -->