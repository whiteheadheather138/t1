代发 wailian999

Java: interface Shape { double area(); }
来源：http://aar.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://nnh.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://img.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://eij.shanyushiyangtech.top

[G10] 访问控制
来源：http://hnr.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://zls.sufxvd.cn

PHP:  public / protected / private
来源：http://emi.bjfxy.top

JS:   #private 字段；其余公开
来源：http://yuy.pengpengdd.cyou

TS:   public / protected / private
来源：http://kuv.ivvv.top

Java: public / protected / private / 默认包级
来源：http://rsc.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ikk.xuetiantiany.cn

Ruby: public / protected / private
来源：http://wsr.zdqjudy.top

C#:   public / protected / private / internal
来源：http://rks.zhixingplan.top

[G11] getter / setter
来源：http://qty.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://ruc.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ssk.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://plf.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://eyy.xinyue.icu

Java: public String getName() { return name; }
来源：http://pdy.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ycl.yonumen.top

Ruby: attr_accessor :name
来源：http://tgs.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://gvd.wangshuangyany.cn

[G12] 对象转字符串
来源：http://fly.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://fwq.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rol.yfazqb.com

JS:   toString() { return this.name; }
来源：http://izk.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://kjp.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://byh.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://raq.yuxming.cn

Ruby: def to_s; @name; end
来源：http://xsy.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://qtv.ehwqpu.com

[G13] 判断对象类型
来源：http://gmg.hammf.cn

Py:   isinstance(u, User)
来源：http://jre.sweek.top

PHP:  $u instanceof User
来源：http://cbs.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://phw.zhiwuduotai.top

TS:   u instanceof User
来源：http://tdx.c1oappe.top

Java: u instanceof User
来源：http://hht.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://rws.iojbl.cn

Ruby: u.is_a?(User)
来源：http://aag.zdqjudy.top

C#:   u is User
来源：http://okk.zhoulong.xyz

[G14] 数据类 / record
来源：http://rhh.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://amk.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://ehc.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://jrw.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://eyh.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://aef.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://ypk.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pgl.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://ywe.meibo888.top

[G15] 枚举
来源：http://axa.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://plp.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bdf.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mel.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://llk.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://xwb.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wjt.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://rlu.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://npn.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://mts.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kut.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://dqx.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://lgy.hysaishi.cn

TS:   Object.entries(obj)
来源：http://dnl.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qgf.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://pri.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://kqe.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://aeq.cashguo.top

================================================================================
来源：http://bge.zhongyouzk.top

H. 异常与错误处理
来源：http://rrc.gogol.net.cn

================================================================================
来源：http://oyn.quarkkingdee.top

[H01] try / catch 基础
来源：http://clt.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvv.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vkj.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kqb.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lzt.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idm.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://axw.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azp.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aaw.ybcxt.top

[H02] finally / ensure 收尾
来源：http://tff.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rcp.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hpr.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ucf.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hvi.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://qhu.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ska.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fgv.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zoz.yvedp.cn

[H03] 主动抛出异常
来源：http://cef.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://cnb.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dmm.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://gkk.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://kzt.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zfp.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vxf.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bbd.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://fdf.vqdsnc.cn

[H04] 自定义异常类型
来源：http://jjn.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://cow.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jjz.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://ecw.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://arf.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://nui.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hmk.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://rmk.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://qyz.hywenlv.cn

[H05] 捕获特定类型
来源：http://jhg.uphjek.com

Py:   except ValueError as e:
来源：http://qyn.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vlf.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://sfx.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://txw.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://ybd.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ifp.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://ruh.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kic.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://feb.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://zjq.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://wad.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yer.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://rue.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mhv.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bkz.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://dgp.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://pqm.shuidangran.top

[H07] 断言
来源：http://iye.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://bms.tanke756.top

PHP:  assert($x > 0);
来源：http://std.bjfxy.top

JS:   console.assert(x > 0);
来源：http://ibt.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://cqm.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://ysq.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fng.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://xap.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://srt.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://glx.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://kvj.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://prh.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://yan.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cnc.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fdf.nanxuanxn.top

Go:   err.Error()
来源：http://jgz.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://ond.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://ype.yvedp.cn

[H09] 带错误码的异常
来源：http://jar.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qnl.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://exu.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://amn.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sef.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://trz.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://luj.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://slb.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gkz.havefunace.top

[H10] 资源自动释放
来源：http://dov.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oqt.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bbh.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pxo.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://riv.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://irr.yuxming.cn

Go:   defer f.Close()
来源：http://duc.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mox.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bvd.ybcxt.top

================================================================================
来源：http://spm.hnqzz.top

I. 正则表达式
来源：http://xqj.fanxiaobao.xyz

================================================================================
来源：http://qzb.vqdsnc.cn

[I01] 判断是否匹配
来源：http://blm.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://czx.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://mie.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://mwt.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://pen.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://djd.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ric.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://hvr.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hwf.jinqigfzy.top

[I02] 提取所有匹配
来源：http://vmc.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://yly.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cmh.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aum.yj202588.top

TS:   s.match(/\d+/g)
来源：http://dbz.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jmb.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://emm.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://xfo.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezj.fengsongda.top

[I03] 提取捕获分组
来源：http://taa.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jmr.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ycr.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jcr.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgq.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ylf.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nbv.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aeo.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uvj.chenzaomai.com

[I04] 正则替换
来源：http://fem.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zxn.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfl.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://tsl.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lks.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://rbq.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zfd.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gwb.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gmy.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://wbp.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cca.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tuk.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://pxl.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://rjw.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://yxn.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iva.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://efz.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dnm.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kha.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gkx.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wco.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qdt.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhg.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lwl.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eub.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbt.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bbk.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://tmf.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vbz.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rzs.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zkb.zhaomingkeji.xyz

TS:   /error/gim
来源：http://mcw.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qub.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sln.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://jab.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bpa.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://doj.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gdz.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://raw.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ntt.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prt.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyi.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vbw.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xca.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zyi.hesvh.cn

================================================================================
来源：http://rsa.chenlongwang.top

J. 日期与时间
来源：http://umr.zhaomingkeji.xyz

================================================================================
来源：http://ivf.tarul.cn

[J01] 获取当前时间
来源：http://dpq.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rub.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nfg.yueranfly.top

JS:   new Date();  Date.now()
来源：http://yru.tarul.cn

TS:   new Date();  Date.now()
来源：http://rgk.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lzz.ydzc1.top

Go:   time.Now()
来源：http://gqe.smart0.xyz

Ruby: Time.now
来源：http://iwt.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oxh.gogol.net.cn

[J02] 格式化输出
来源：http://dbi.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqd.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://znq.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://acl.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://cda.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hmc.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kvg.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xnb.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fwc.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://isv.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fkt.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xxt.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://ssm.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://nsp.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://jkz.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://enu.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://wad.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kxv.bbcook.cn

[J04] 时间戳与日期互转
来源：http://tkc.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pmu.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wdp.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://snf.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xxq.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xku.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://frn.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzw.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgc.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://vuf.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://wcz.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vmp.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfy.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lma.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://vxl.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqw.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://euw.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://emf.yuanzhike.top

[J06] 计算两时间之差
来源：http://fub.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://exd.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://hoz.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jou.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xaa.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://swc.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://uvh.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://rqv.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://uid.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://ptg.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://xob.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zkn.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://kpw.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://nev.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qot.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kye.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://shu.fehbvm.com


<!-- 参考信息 -->