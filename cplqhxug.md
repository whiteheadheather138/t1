代发 wailian999

C#:   public / protected / private / internal
来源：http://qom.zhengqikj.top

[G11] getter / setter
来源：http://tmr.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://ijt.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nxn.yj202588.top

JS:   get name() { return this._name; }
来源：http://jcy.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://zrs.jqgfzy.top

Java: public String getName() { return name; }
来源：http://oap.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pet.hesvh.cn

Ruby: attr_accessor :name
来源：http://ogg.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://hsk.jlsjyb.cn

[G12] 对象转字符串
来源：http://jvy.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://anb.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zfm.aizwys.cn

JS:   toString() { return this.name; }
来源：http://azd.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://uaf.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://wvd.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zqu.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://pnv.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://qid.snrcjt.cn

[G13] 判断对象类型
来源：http://pec.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://via.daxiang520.top

PHP:  $u instanceof User
来源：http://ktf.c1oappe.top

JS:   u instanceof User
来源：http://juc.yueranfly.top

TS:   u instanceof User
来源：http://gqy.chenjidiqi.icu

Java: u instanceof User
来源：http://dvm.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dmj.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://zov.gogol.net.cn

C#:   u is User
来源：http://cvl.nwbrower.top

[G14] 数据类 / record
来源：http://xnd.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bso.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://glg.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lae.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://xvp.yonumen.top

Java: record User(String name, int age) {}
来源：http://usk.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://krn.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://abn.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://uyn.sufxvd.cn

[G15] 枚举
来源：http://cxp.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jey.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ezy.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eka.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://auu.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://vip.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wse.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://hqy.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oqw.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://yeh.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wtg.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://yhm.hnqzz.top

JS:   Object.entries(obj)
来源：http://wss.jiagoushi.top

TS:   Object.entries(obj)
来源：http://crh.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ifp.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://eda.smart0.xyz

Ruby: obj.instance_variables
来源：http://yds.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://rdy.hysaishi.cn

================================================================================
来源：http://krj.nwbrower.top

H. 异常与错误处理
来源：http://smo.ydzc1.top

================================================================================
来源：http://jqt.andypj.xyz

[H01] try / catch 基础
来源：http://tcu.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://owk.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lsv.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://udn.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://itd.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://poj.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hej.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rdd.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mlr.cucudq.cn

[H02] finally / ensure 收尾
来源：http://upk.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lgn.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zkz.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oom.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lno.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ozt.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhl.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kch.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://een.daria6918.cn

[H03] 主动抛出异常
来源：http://odt.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://ufw.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gus.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://pgv.316326.xyz

TS:   throw new Error("错误信息");
来源：http://uyr.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iab.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://icl.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qbg.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://jws.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://jmz.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://xit.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://gad.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://tss.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://rff.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://usl.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dxp.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://uzd.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://hjg.yongpay.top

[H05] 捕获特定类型
来源：http://raz.316326.xyz

Py:   except ValueError as e:
来源：http://xwx.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wju.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://sca.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://ixr.ehwqpu.com

Java: catch (IOException | SQLException e) {}
来源：http://wdt.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hcc.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://rau.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ddp.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://lst.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://ajo.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vvm.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bsd.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://iyj.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wvd.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://okp.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://krx.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://qtg.andypj.xyz

[H07] 断言
来源：http://wjj.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://xts.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://afc.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://gqi.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://jfn.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://jag.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ajl.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nqs.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://dea.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://hcj.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://quq.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbf.iojbl.cn

JS:   e.message;  e.stack
来源：http://fns.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xlc.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qtx.ctjpmb.com

Go:   err.Error()
来源：http://tdt.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://aus.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://klb.cucudq.cn

[H09] 带错误码的异常
来源：http://vhc.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rwp.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://khb.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mtt.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tof.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://leg.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://glu.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://acd.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://orx.zhongyouzk.top

[H10] 资源自动释放
来源：http://utx.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mlc.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://igz.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ufl.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dir.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgg.jiagoushi.top

Go:   defer f.Close()
来源：http://cdo.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ppo.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ujx.yuanzhike.top

================================================================================
来源：http://ytl.yj202588.top

I. 正则表达式
来源：http://ubo.jianghu66.top

================================================================================
来源：http://vgu.hfpthk.cn

[I01] 判断是否匹配
来源：http://bzo.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ams.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://aay.epnwcf.com

JS:   /\d+/.test(s)
来源：http://bbx.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://gre.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvn.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xzv.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://eui.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ort.chenzaomai.com

[I02] 提取所有匹配
来源：http://nji.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://dbh.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://saq.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lty.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://cfb.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pne.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hsc.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://gpd.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ujr.fengsongda.top

[I03] 提取捕获分组
来源：http://sfe.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ifc.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://phk.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zug.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zhh.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iig.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfw.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ihz.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gql.yfazqb.com

[I04] 正则替换
来源：http://bef.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://szu.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nyu.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://zbi.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://tva.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://ape.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ktd.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://nqf.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://irz.cdnleiting.top

[I05] 按正则拆分
来源：http://hpt.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://nug.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://irp.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://pel.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://sys.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://dou.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cab.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iww.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ubk.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qtu.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dxh.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rby.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ehf.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vcs.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://efg.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fkj.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lyo.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zpz.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://xmf.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ror.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aeg.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kus.sxryk.cn

TS:   /error/gim
来源：http://syt.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kys.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blu.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://lfj.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lgl.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://jlm.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ary.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fem.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gos.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iat.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://pyy.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nrs.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qyq.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fsm.xinyue.icu

================================================================================
来源：http://ayy.dianchejie.cn

J. 日期与时间
来源：http://ibf.hywenlv.cn

================================================================================
来源：http://bgl.yueranfly.top

[J01] 获取当前时间
来源：http://lly.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://okh.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cnu.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://afw.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://wxj.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tbb.svipenyu.cn

Go:   time.Now()
来源：http://flp.xziqi.cn

Ruby: Time.now
来源：http://dih.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oev.nwbrower.top

[J02] 格式化输出
来源：http://ceg.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdo.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rgz.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://apc.bbcook.cn

TS:   d.toISOString()
来源：http://wky.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rlb.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://son.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zki.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tom.nanxinkj.top

[J03] 字符串解析为日期
来源：http://dgb.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xce.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jyr.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://ekc.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://eia.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zpc.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zul.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://nhi.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iod.zycfv.cn

[J04] 时间戳与日期互转
来源：http://qwj.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ktj.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ysd.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://edg.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tzn.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ila.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xmh.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dhp.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://apf.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://zaf.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://fza.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xmv.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rfl.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://imv.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://oba.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jen.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://ywi.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://lcv.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://krf.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://obc.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://qaf.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fzh.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lpz.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://kkn.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://tcn.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://ood.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://ydz.jianghu66.top

[J07] 比较两个日期
来源：http://bdy.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://ggw.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xqv.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lfy.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://txk.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qls.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://suj.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ezv.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://req.xziqi.cn

[J08] 提取年月日与星期
来源：http://twa.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://djg.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dyh.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bea.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jkg.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fpf.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rfa.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://grf.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dsj.redwolf501.top

[J09] 时区处理
来源：http://nrz.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jvb.jinghuilouyu.cn


<!-- 参考信息 -->