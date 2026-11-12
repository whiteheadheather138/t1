代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://tgs.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://ghp.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qii.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://luz.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://puw.epnwcf.com

[G07] 调用父类方法
来源：http://coi.feifeiyinyue.top

Py:   super().greet()
来源：http://qbw.chenlongwang.top

PHP:  parent::greet();
来源：http://ler.vehdjk.com

JS:   super.greet();
来源：http://phi.dianchejie.cn

TS:   super.greet();
来源：http://khr.zdqjudy.top

Java: super.greet();
来源：http://nxa.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xas.zdbjq.cn

Ruby: super
来源：http://iuw.sweek.top

C#:   base.Greet();
来源：http://ive.daxiang520.top

[G08] 静态方法与属性
来源：http://rse.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fbm.fzhhl.top

PHP:  public static function f() {}
来源：http://fsh.ppjwa.cn

JS:   static f() {}
来源：http://aoa.wangdashe.top

TS:   static f(): void {}
来源：http://wnv.shuidangran.top

Java: static void f() {}
来源：http://zbh.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rhf.yj202588.top

Ruby: def self.f; end
来源：http://nqu.shzxlz.cn

C#:   public static void F() {}
来源：http://nfs.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://yji.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://ubh.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://lbi.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ndx.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://dbi.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://vod.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://gzt.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://inu.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://jhp.shanyushiyangkeji.top

[G10] 访问控制
来源：http://itq.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://poe.xuanzx.com

PHP:  public / protected / private
来源：http://jzp.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://bsz.mhx1999.top

TS:   public / protected / private
来源：http://qor.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://hxz.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rnz.cashguo.top

Ruby: public / protected / private
来源：http://fju.ctjpmb.com

C#:   public / protected / private / internal
来源：http://ntu.svipenyu.cn

[G11] getter / setter
来源：http://qsm.yj20258.top

Py:   @property 与 @x.setter
来源：http://qxe.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jov.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://rws.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://dgr.jyoumei.cn

Java: public String getName() { return name; }
来源：http://kvk.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ktf.tian-w.cn

Ruby: attr_accessor :name
来源：http://ozf.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://vih.jiagoushi.top

[G12] 对象转字符串
来源：http://kzf.tanke756.top

Py:   def __str__(self): return self.name
来源：http://pvd.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://myz.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://pxk.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://uql.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://euw.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://rbi.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://cpr.tarul.cn

C#:   public override string ToString() => Name;
来源：http://knl.yfazqb.com

[G13] 判断对象类型
来源：http://vgd.yuxming.cn

Py:   isinstance(u, User)
来源：http://nrf.aizwys.cn

PHP:  $u instanceof User
来源：http://zaz.shzxlz.cn

JS:   u instanceof User
来源：http://nlg.52xcode.cn

TS:   u instanceof User
来源：http://vni.yfazqb.com

Java: u instanceof User
来源：http://bpy.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xek.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://ual.zhengqikj.top

C#:   u is User
来源：http://spx.shangyingyoupin.top

[G14] 数据类 / record
来源：http://vrn.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zog.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://wcg.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://krh.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://otm.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://pig.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://nro.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bjm.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://qny.xuanzx.com

[G15] 枚举
来源：http://rom.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pnr.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vzb.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wxh.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fye.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://jar.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xsv.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://nbi.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xrr.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://gkz.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zwi.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://gyk.9152youxi.cn

JS:   Object.entries(obj)
来源：http://rrr.ybcxt.top

TS:   Object.entries(obj)
来源：http://wrh.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hma.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bew.tianlin.xyz

Ruby: obj.instance_variables
来源：http://zno.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://tbk.fehbvm.com

================================================================================
来源：http://jwc.tarul.cn

H. 异常与错误处理
来源：http://ktb.yvedp.cn

================================================================================
来源：http://mzk.jianghu66.top

[H01] try / catch 基础
来源：http://qrs.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://llv.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cwq.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tjc.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://foe.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://emo.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://weg.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yjb.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lev.aizwys.cn

[H02] finally / ensure 收尾
来源：http://xjn.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://flv.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://viq.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ooo.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jlf.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://xvx.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ldw.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kfr.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ajz.hammf.cn

[H03] 主动抛出异常
来源：http://fmb.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://wfu.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgc.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://ttc.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://des.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zts.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fhu.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mcv.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://rmm.jyoumei.cn

[H04] 自定义异常类型
来源：http://ooq.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://ahb.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://wgr.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://juu.xuanzx.com

TS:   class MyError extends Error {}
来源：http://rmp.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://otv.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ysv.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://ynw.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://oyy.ivvv.top

[H05] 捕获特定类型
来源：http://pgi.epnwcf.com

Py:   except ValueError as e:
来源：http://may.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mmr.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://dgb.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://hfm.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://pzz.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xux.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://mgn.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fzv.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://uri.hesvh.cn

Py:   value = d.get("k") or default
来源：http://gtn.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://dtj.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://llq.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://prv.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xdl.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iam.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://bkw.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://hfo.bjfxy.top

[H07] 断言
来源：http://zzp.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://sgb.mhx1999.top

PHP:  assert($x > 0);
来源：http://dxs.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://xsw.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://trk.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://zwd.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tqu.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xvt.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://flr.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://rov.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://tsf.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vgm.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://wkx.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pxv.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yqd.shanyushiyangtech.top

Go:   err.Error()
来源：http://ybx.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://gzz.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://eox.daria6918.cn

[H09] 带错误码的异常
来源：http://wmd.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pph.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bmx.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tan.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ubv.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://scz.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ukx.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zgs.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zdw.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://bza.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gec.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tni.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jvk.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vuv.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lql.fzhhl.top

Go:   defer f.Close()
来源：http://pfq.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fux.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxj.fzhhl.top

================================================================================
来源：http://pef.xziqi.cn

I. 正则表达式
来源：http://uyo.sjlbkw.cn

================================================================================
来源：http://rbg.jianghu66.top

[I01] 判断是否匹配
来源：http://swx.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdp.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ids.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://nki.wangdashe.top

TS:   /\d+/.test(s)
来源：http://vni.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wsi.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xle.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://nxl.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rwy.sufxvd.cn

[I02] 提取所有匹配
来源：http://mxe.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://vty.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://slh.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phv.pycfn.com

TS:   s.match(/\d+/g)
来源：http://sbh.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fqu.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rru.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://qeb.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ejy.zhoulong.xyz

[I03] 提取捕获分组
来源：http://nsu.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hbw.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jbh.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wbs.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wet.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uku.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://stt.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://faa.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dpq.zhengqikj.top

[I04] 正则替换
来源：http://kod.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tek.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zkp.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://gtd.yongpay.top

TS:   s.replace(/\d+/g, "#")
来源：http://mrt.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://evn.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wqv.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oop.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kib.smart0.xyz

[I05] 按正则拆分
来源：http://yzx.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://det.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zrc.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://lep.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://rmc.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://lsv.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vgw.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bex.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sco.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vpg.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://spb.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jjp.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wyb.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxv.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vew.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bob.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ohl.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zck.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://rmm.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oiw.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vtr.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dvb.wangshuangyany.cn

TS:   /error/gim
来源：http://vqw.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kos.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ana.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://hpp.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ltn.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://pew.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sjm.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://imu.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xcl.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nhb.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xgo.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://api.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eqt.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iyq.fengsongda.top

================================================================================
来源：http://mhj.jinghuilouyu.cn

J. 日期与时间
来源：http://uum.jqgufenzy.top

================================================================================
来源：http://rto.haohaochexian.top

[J01] 获取当前时间
来源：http://dkg.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jbz.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdl.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://pak.pycfn.com

TS:   new Date();  Date.now()
来源：http://tgb.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://drt.zdqjudy.top

Go:   time.Now()
来源：http://zgo.dianchejie.cn

Ruby: Time.now
来源：http://orh.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihc.shuidangran.top

[J02] 格式化输出
来源：http://ino.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oeo.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mrp.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mfd.pengpengdd.cyou

TS:   d.toISOString()
来源：http://yko.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lzh.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pja.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlu.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pxm.9152youxi.cn

[J03] 字符串解析为日期
来源：http://zsi.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gxd.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dbi.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://usl.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://gdm.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://psl.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fzc.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://kck.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://soa.tian-w.cn

[J04] 时间戳与日期互转
来源：http://jaz.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iju.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fbo.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ifb.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vyu.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ped.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://txt.hammf.cn


<!-- 参考信息 -->