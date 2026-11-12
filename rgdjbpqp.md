代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://gkd.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zni.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ilh.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://rte.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://enx.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://vzm.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://psi.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://ifm.sufxvd.cn

[G10] 访问控制
来源：http://bzw.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://qdm.birdmap.top

PHP:  public / protected / private
来源：http://qyj.aizwys.cn

JS:   #private 字段；其余公开
来源：http://cwl.zycfv.cn

TS:   public / protected / private
来源：http://oro.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://qyq.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hpd.daxiang520.top

Ruby: public / protected / private
来源：http://ehg.gzhubu.top

C#:   public / protected / private / internal
来源：http://mrp.ydzc1.top

[G11] getter / setter
来源：http://cgq.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://iwn.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kzc.yvedp.cn

JS:   get name() { return this._name; }
来源：http://gog.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://bvl.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://icv.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yuc.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://mhx.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://rup.kuanghao11.cn

[G12] 对象转字符串
来源：http://zen.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://vjs.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vjk.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://dqo.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://usx.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://nuk.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eea.guannengcc.top

Ruby: def to_s; @name; end
来源：http://rwx.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://akl.xinyue.icu

[G13] 判断对象类型
来源：http://rqq.sysykeji.top

Py:   isinstance(u, User)
来源：http://zud.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://gvw.cqqwz.cn

JS:   u instanceof User
来源：http://uik.jqgufenzy.top

TS:   u instanceof User
来源：http://dvv.xuetiantiany.cn

Java: u instanceof User
来源：http://vik.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rbd.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://eyx.sysykeji.top

C#:   u is User
来源：http://otz.hcnkem.com

[G14] 数据类 / record
来源：http://bfb.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xgs.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ude.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://udp.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://std.316326.xyz

Java: record User(String name, int age) {}
来源：http://rgj.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://ydx.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://izt.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://oah.yuxming.cn

[G15] 枚举
来源：http://hem.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://djh.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbu.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ywp.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kxm.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://xfn.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://evd.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://itt.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://igz.yongpay.top

[G16] 对象转数组 / 字典
来源：http://hal.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mre.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://ppd.cdnleiting.top

JS:   Object.entries(obj)
来源：http://wjd.zdqjudy.top

TS:   Object.entries(obj)
来源：http://fhq.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dcy.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cpi.jiagoushi.top

Ruby: obj.instance_variables
来源：http://xgj.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://vru.meibo888.top

================================================================================
来源：http://zwf.meibo888.top

H. 异常与错误处理
来源：http://pfj.dianchejie.cn

================================================================================
来源：http://fzs.daria6918.cn

[H01] try / catch 基础
来源：http://gys.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://akm.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mtk.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uiv.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rjt.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afc.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xcm.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fcr.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bfk.yj202588.top

[H02] finally / ensure 收尾
来源：http://yqd.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://god.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mib.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ter.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vxk.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://ecv.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tpw.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yir.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpr.shuidangran.top

[H03] 主动抛出异常
来源：http://nyc.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://ymy.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://doo.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://gle.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://iyu.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zkb.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://loc.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pww.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://uzs.zhongyouzk.top

[H04] 自定义异常类型
来源：http://jli.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://loe.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lar.c1oappe.top

JS:   class MyError extends Error {}
来源：http://zni.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://npd.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://fxy.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hwv.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://uff.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://myh.havefunace.top

[H05] 捕获特定类型
来源：http://oza.redwolf501.top

Py:   except ValueError as e:
来源：http://ykj.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qzg.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://amb.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://sos.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://lsv.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvz.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://ewd.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qcd.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://mqn.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://eld.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vom.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://pmc.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://blr.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fap.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iit.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://vsi.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://cmw.nanxinkj.top

[H07] 断言
来源：http://kvp.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://gxf.shzxlz.cn

PHP:  assert($x > 0);
来源：http://atk.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://tct.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://bin.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://het.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vyu.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://iou.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://soj.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://wqh.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://qvr.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tgi.guannengcc.top

JS:   e.message;  e.stack
来源：http://eay.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nhw.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ilq.svipenyu.cn

Go:   err.Error()
来源：http://iaz.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://esp.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://kgu.hnqzz.top

[H09] 带错误码的异常
来源：http://duw.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wxp.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xvr.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ltl.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ilh.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uuo.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jut.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://qwi.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qxe.sweek.top

[H10] 资源自动释放
来源：http://bui.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cti.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://evp.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uwp.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iya.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gcc.jqgfzy.top

Go:   defer f.Close()
来源：http://xgb.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ibc.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebt.fktsv.cn

================================================================================
来源：http://fwc.jinqigufen.top

I. 正则表达式
来源：http://nhm.ywan-chungtsiang.top

================================================================================
来源：http://yqw.yj20258888.top

[I01] 判断是否匹配
来源：http://iql.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vee.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ltd.tian-w.cn

JS:   /\d+/.test(s)
来源：http://kpr.shuidangran.top

TS:   /\d+/.test(s)
来源：http://rif.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qlc.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jor.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://wip.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://upz.ppjwa.cn

[I02] 提取所有匹配
来源：http://rto.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://ocs.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kou.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xkp.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://upe.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ova.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sxb.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://owy.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nxk.bbcook.cn

[I03] 提取捕获分组
来源：http://ufs.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sly.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yba.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gis.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cqg.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lpj.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://llr.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iny.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qvp.jinqigufen.top

[I04] 正则替换
来源：http://fqq.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://wet.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tpj.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://zsi.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://sub.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://zxo.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://qsb.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jmf.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://van.xziqi.cn

[I05] 按正则拆分
来源：http://mzp.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gqh.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hcb.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://pdh.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://ims.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://xrg.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qgq.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://giv.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zkn.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wvv.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vej.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hyj.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uhv.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yol.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zyn.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tio.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nkp.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ent.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://jnv.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ket.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fxf.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ixw.cashguo.top

TS:   /error/gim
来源：http://loe.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gdg.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://llr.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://xdt.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bxz.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://oqq.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mow.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pvm.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpk.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://edu.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ddx.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fiu.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zae.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://odt.meibo888.top

================================================================================
来源：http://nmw.9152youxi.cn

J. 日期与时间
来源：http://qqe.shangyingyoupin.top

================================================================================
来源：http://mxh.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://lan.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ozy.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xvb.fktsv.cn

JS:   new Date();  Date.now()
来源：http://mai.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://tkn.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://swi.shuidangran.top

Go:   time.Now()
来源：http://mxy.svipenyu.cn

Ruby: Time.now
来源：http://vnf.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nxx.yongpay.top

[J02] 格式化输出
来源：http://mgo.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jey.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jcq.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wcm.chenlongwang.top

TS:   d.toISOString()
来源：http://yeq.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uya.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://llw.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://irf.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://npn.ydzc1.top

[J03] 字符串解析为日期
来源：http://uui.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bqj.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fod.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://krl.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://gel.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fzy.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzu.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://pcf.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qvq.yongpay.top

[J04] 时间戳与日期互转
来源：http://mvp.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pir.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://onz.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oxz.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bce.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ehy.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mxx.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vmf.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kcg.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://bhx.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://yft.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnk.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwh.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pjk.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://rkr.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amm.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://vta.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://abz.yuxming.cn

[J06] 计算两时间之差
来源：http://ugc.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://ocv.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://css.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kra.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lyy.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://bba.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://ajd.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://flt.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://zca.aizwys.cn

[J07] 比较两个日期
来源：http://cot.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://xfh.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khf.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jbl.jqgfzy.top


<!-- 参考信息 -->