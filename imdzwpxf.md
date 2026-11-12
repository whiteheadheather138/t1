代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://qjj.xuanzx.com

Ruby: def self.f; end
来源：http://pib.sufxvd.cn

C#:   public static void F() {}
来源：http://upl.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://wfl.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://cep.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://fqf.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uyk.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://bsl.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://mjq.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://tjy.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mav.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://jtd.ppjwa.cn

[G10] 访问控制
来源：http://eah.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://flw.xylfe.cn

PHP:  public / protected / private
来源：http://hju.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://xaq.yonumen.top

TS:   public / protected / private
来源：http://umy.pycfn.com

Java: public / protected / private / 默认包级
来源：http://yvt.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvh.guowangkeji.top

Ruby: public / protected / private
来源：http://fsa.gzhubu.top

C#:   public / protected / private / internal
来源：http://ccv.cdnleiting.top

[G11] getter / setter
来源：http://fws.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://ofg.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cre.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://sbj.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://jek.svipenyu.cn

Java: public String getName() { return name; }
来源：http://adq.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwn.havefunace.top

Ruby: attr_accessor :name
来源：http://mgf.bbcook.cn

C#:   public string Name { get; set; }
来源：http://rqv.zhixingplan.top

[G12] 对象转字符串
来源：http://aln.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://ebw.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://gea.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://ooh.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://ock.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://drz.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://gqy.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://knf.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://hvx.316326.xyz

[G13] 判断对象类型
来源：http://osm.hysaishi.cn

Py:   isinstance(u, User)
来源：http://nyr.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://rsc.shzxlz.cn

JS:   u instanceof User
来源：http://rub.jinqigfzy.top

TS:   u instanceof User
来源：http://kix.ywan-chungtsiang.top

Java: u instanceof User
来源：http://fid.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nzt.zycfv.cn

Ruby: u.is_a?(User)
来源：http://jif.meibo888.top

C#:   u is User
来源：http://axh.hnqzz.top

[G14] 数据类 / record
来源：http://meu.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fej.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://rqk.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oeq.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://obz.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://tqe.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://ztv.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kda.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://jnf.aibaodan.cn

[G15] 枚举
来源：http://gxv.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eke.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://thd.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mta.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ofa.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://ssk.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rwu.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://efb.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tuh.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://aux.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://stq.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://jjv.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://zgg.zhixingplan.top

TS:   Object.entries(obj)
来源：http://ogu.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jcs.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fix.aibaodan.cn

Ruby: obj.instance_variables
来源：http://gli.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://wdy.chenzaomai.com

================================================================================
来源：http://epq.tianlin.xyz

H. 异常与错误处理
来源：http://pvo.cqqwz.cn

================================================================================
来源：http://nem.pengpengdd.cyou

[H01] try / catch 基础
来源：http://soq.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eye.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://npu.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ilg.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fcl.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ocd.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ouv.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cut.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qrb.bbcook.cn

[H02] finally / ensure 收尾
来源：http://lat.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://div.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hvz.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xmq.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ejb.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wpo.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vnt.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zph.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhk.zycfv.cn

[H03] 主动抛出异常
来源：http://grv.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://ofs.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oyg.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://wrx.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://lla.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ooh.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://imb.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://swp.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://mcm.andypj.xyz

[H04] 自定义异常类型
来源：http://hmu.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://upx.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://boj.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://lgj.hammf.cn

TS:   class MyError extends Error {}
来源：http://bny.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://xev.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bpb.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://qax.guannengcc.top

C#:   class MyException : Exception {}
来源：http://ugy.zhengqikj.top

[H05] 捕获特定类型
来源：http://ooc.zdqjudy.top

Py:   except ValueError as e:
来源：http://vwg.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cus.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://oct.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://thw.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://qjl.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uca.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://vca.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ftx.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://phz.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://ans.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uue.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rui.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://jhe.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qjs.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://quo.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://ezf.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://fpr.tarul.cn

[H07] 断言
来源：http://vhe.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://hlk.ehwqpu.com

PHP:  assert($x > 0);
来源：http://zyd.daria6918.cn

JS:   console.assert(x > 0);
来源：http://ueh.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://cgw.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://vyf.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sgj.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://tda.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://dzv.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://qpw.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://oyv.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qgi.0kj1m.cn

JS:   e.message;  e.stack
来源：http://ftv.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tlt.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mbd.zhongyouzk.top

Go:   err.Error()
来源：http://dqt.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://xas.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://znu.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://lzz.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uun.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jam.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vgk.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nmi.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tox.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vki.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://kua.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ndm.xuanzx.com

[H10] 资源自动释放
来源：http://elj.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rxv.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eky.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://six.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://amh.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jok.ydjk.org.cn

Go:   defer f.Close()
来源：http://ghm.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pls.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sbm.0kj1m.cn

================================================================================
来源：http://npa.sweek.top

I. 正则表达式
来源：http://lnb.aizwys.cn

================================================================================
来源：http://fng.haohaochexian.top

[I01] 判断是否匹配
来源：http://crv.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://idb.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://pti.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://avs.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://tkx.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jas.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nhg.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://sor.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ggw.jinqigufen.top

[I02] 提取所有匹配
来源：http://lhl.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://gqj.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jig.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phe.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://ngb.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dts.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rop.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://xuo.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ysl.chenzaomai.com

[I03] 提取捕获分组
来源：http://fsf.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oli.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gls.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fey.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rwl.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eak.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uuk.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pvw.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mct.wangshuangyany.cn

[I04] 正则替换
来源：http://ejq.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jip.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rsh.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://ory.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qbk.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://wez.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zav.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sgz.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qgs.ydzc1.top

[I05] 按正则拆分
来源：http://izx.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sap.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mar.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://dnm.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://tlu.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://haw.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rgj.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://usx.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ivx.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cmw.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oub.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fuj.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyu.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpn.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wof.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gru.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yup.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ort.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://bor.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://adx.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmr.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfb.yvedp.cn

TS:   /error/gim
来源：http://vpc.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tan.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xah.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://ayf.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wgh.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://sua.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nvz.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hrd.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzc.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ket.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://lbe.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cwz.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bkb.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://stm.aizwys.cn

================================================================================
来源：http://vgr.0kj1m.cn

J. 日期与时间
来源：http://yat.yvedp.cn

================================================================================
来源：http://rds.yfazqb.com

[J01] 获取当前时间
来源：http://pps.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xnh.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fhk.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://qsp.aizwys.cn

TS:   new Date();  Date.now()
来源：http://adn.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://upo.shzxlz.cn

Go:   time.Now()
来源：http://kxl.xuanzx.com

Ruby: Time.now
来源：http://bxh.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://del.feifeiyinyue.top

[J02] 格式化输出
来源：http://rab.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qgg.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://naf.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgm.zhongyouzk.top

TS:   d.toISOString()
来源：http://eek.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eze.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fkc.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bnm.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://orf.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://kih.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cqw.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qiu.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://vvy.cheryme.top

TS:   new Date("2024-01-02")
来源：http://zab.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://cif.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tls.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://uax.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vns.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://dby.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://leh.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ocf.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://obl.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://stl.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nhk.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vwi.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfr.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kfj.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://nwo.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://etq.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://olu.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwb.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gri.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://kwj.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iza.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://ptf.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://zwd.sysykeji.top

[J06] 计算两时间之差
来源：http://ymy.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://ajo.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://fup.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uno.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tvr.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://uqk.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://yjq.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://dhf.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://mnd.guannengcc.top


<!-- 参考信息 -->