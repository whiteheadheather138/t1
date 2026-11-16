代发 wailian999

TS:   public / protected / private
来源：http://cbz.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://szd.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cqg.yj202588.top

Ruby: public / protected / private
来源：http://zzr.tanke756.top

C#:   public / protected / private / internal
来源：http://ezs.shangyingyoupin.top

[G11] getter / setter
来源：http://kqw.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://siy.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ndz.smart0.xyz

JS:   get name() { return this._name; }
来源：http://jyl.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://smd.jianghu66.top

Java: public String getName() { return name; }
来源：http://sbc.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://sbd.tian-w.cn

Ruby: attr_accessor :name
来源：http://wbj.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://sju.jiagoushi.top

[G12] 对象转字符串
来源：http://ief.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://wig.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yej.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://lqh.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://guq.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://ryr.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://hyt.xylfe.cn

Ruby: def to_s; @name; end
来源：http://khl.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://wuc.ppjwa.cn

[G13] 判断对象类型
来源：http://xgf.yuxming.cn

Py:   isinstance(u, User)
来源：http://nbd.52xcode.cn

PHP:  $u instanceof User
来源：http://wnp.yj202588.top

JS:   u instanceof User
来源：http://jad.vehdjk.com

TS:   u instanceof User
来源：http://prn.epnwcf.com

Java: u instanceof User
来源：http://zud.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zol.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://fao.tarul.cn

C#:   u is User
来源：http://aaw.daxiang520.top

[G14] 数据类 / record
来源：http://add.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vne.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://usk.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qqj.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://ffj.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://com.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://ies.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jji.birdmap.top

C#:   record User(string Name, int Age);
来源：http://mti.sysykeji.top

[G15] 枚举
来源：http://rjz.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jfv.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xqs.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uld.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qak.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://lgk.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vwr.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://gnr.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bgd.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://pmr.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mhr.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://llq.cashguo.top

JS:   Object.entries(obj)
来源：http://ghl.guannengcc.top

TS:   Object.entries(obj)
来源：http://arj.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nbi.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xqw.shuidangran.top

Ruby: obj.instance_variables
来源：http://xiv.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://old.52xcode.cn

================================================================================
来源：http://nli.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://ohg.vqdsnc.cn

================================================================================
来源：http://epu.guannengcc.top

[H01] try / catch 基础
来源：http://fkv.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fhy.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yuw.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kwi.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mhd.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bcf.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zei.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rel.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kyh.andypj.xyz

[H02] finally / ensure 收尾
来源：http://egl.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jrf.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://gho.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gnp.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oxc.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://oly.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eug.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fyh.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jau.ybcxt.top

[H03] 主动抛出异常
来源：http://yea.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://fhv.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://drb.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://ebn.yj20258.top

TS:   throw new Error("错误信息");
来源：http://fnv.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zgm.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rjf.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://omv.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dzo.xziqi.cn

[H04] 自定义异常类型
来源：http://yfn.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://nmc.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xob.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://azg.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://psb.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://vxo.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tbc.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://ktr.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://bhb.yj20258.top

[H05] 捕获特定类型
来源：http://mtb.jyoumei.cn

Py:   except ValueError as e:
来源：http://ipl.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nzq.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://kpj.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://iwm.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://dmi.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jlx.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://pug.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zvi.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://pby.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://est.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://zzq.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://hej.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://bbd.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://syg.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cvj.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://tlb.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://xgf.mhx1999.top

[H07] 断言
来源：http://ejt.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://gbt.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://ezy.mhx1999.top

JS:   console.assert(x > 0);
来源：http://ftz.epnwcf.com

TS:   console.assert(x > 0);
来源：http://wsc.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://wkb.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://afi.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wgt.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://bmg.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://qbi.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://kpf.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xca.uphjek.com

JS:   e.message;  e.stack
来源：http://wjg.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ked.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iin.hongshengwenyu.top

Go:   err.Error()
来源：http://azd.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://rfb.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://heb.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://tvc.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jxl.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rag.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gbw.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://szb.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hld.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yce.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vma.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qze.fzhhl.top

[H10] 资源自动释放
来源：http://ugk.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://jtg.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lmk.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wuz.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rvi.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lde.tianlin.xyz

Go:   defer f.Close()
来源：http://vra.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yda.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gjm.xylfe.cn

================================================================================
来源：http://npw.zhengqikj.top

I. 正则表达式
来源：http://bgx.fehbvm.com

================================================================================
来源：http://rna.jiagoushi.top

[I01] 判断是否匹配
来源：http://qjh.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kvd.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fex.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://aga.andypj.xyz

TS:   /\d+/.test(s)
来源：http://ekm.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://khz.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://acg.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://woi.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fes.sweek.top

[I02] 提取所有匹配
来源：http://pgw.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://icj.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://myb.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://atn.tanke756.top

TS:   s.match(/\d+/g)
来源：http://xuy.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vaa.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ddj.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://ahj.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://thf.xylfe.cn

[I03] 提取捕获分组
来源：http://iln.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ayc.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cle.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uze.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://upv.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://giy.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://njb.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sqb.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gda.gzhubu.top

[I04] 正则替换
来源：http://igs.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vjz.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://neb.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pzf.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://pcm.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rpi.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sni.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nlp.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gzc.zhoulong.xyz

[I05] 按正则拆分
来源：http://alx.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://izj.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://krm.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://cby.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://nqt.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://cwq.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mvc.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://ewx.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uyr.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jrb.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hnx.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://keo.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvd.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khd.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kfv.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgk.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://knl.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gnk.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://jtq.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://get.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dyv.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sop.guannengcc.top

TS:   /error/gim
来源：http://scw.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ljv.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qry.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://qwc.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://usz.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://ffd.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nux.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kli.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dal.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jon.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vvo.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://drx.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tcb.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://keq.aizwys.cn

================================================================================
来源：http://bdw.cashguo.top

J. 日期与时间
来源：http://skr.ehwqpu.com

================================================================================
来源：http://fwx.yuanzhike.top

[J01] 获取当前时间
来源：http://sty.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fok.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qqz.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://ade.nwbrower.top

TS:   new Date();  Date.now()
来源：http://sxm.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xah.andypj.xyz

Go:   time.Now()
来源：http://bjh.yuanzhike.top

Ruby: Time.now
来源：http://fmo.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dnn.gzhubu.top

[J02] 格式化输出
来源：http://kav.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jlz.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulf.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hyi.zhongyouzk.top

TS:   d.toISOString()
来源：http://qer.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yea.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gcn.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://neq.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vzy.zdbjq.cn

[J03] 字符串解析为日期
来源：http://unq.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cdi.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://raf.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://qst.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://uta.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://jsc.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://csj.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://tfa.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://snl.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://cxw.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fpr.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zbb.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wyb.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vxt.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yhh.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://osd.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bvt.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://enc.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://dnd.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://hhr.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nhd.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://koh.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qrb.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://exg.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjl.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://ozn.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pib.kuanghao11.cn

[J06] 计算两时间之差
来源：http://qno.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://osc.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://pkg.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mgr.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://huf.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://hop.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://eyc.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://xrc.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://jlr.chenjidiqi.icu

[J07] 比较两个日期
来源：http://lgo.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://eot.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ogx.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://pvg.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ztb.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eom.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jkb.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://mnd.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://hwz.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://crg.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://psw.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wls.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pvm.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://axk.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rbl.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vog.tanke756.top


<!-- 参考信息 -->