代发 wailian999

[Q76] 按天统计
来源：http://wcc.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qbg.redwolf501.top

[Q77] 时间加减
来源：http://mnf.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mul.cdnleiting.top

[Q78] 当前时间
来源：http://qzw.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mfi.c1oappe.top

[Q79] 字符串拼接
来源：http://nip.xziqi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uei.nanxinkj.top

[Q80] 字符串截取
来源：http://bnv.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rha.316326.xyz

[Q81] 字符串替换
来源：http://tmz.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mgx.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://bjx.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kfl.xinyue.icu

[Q83] 大小写转换
来源：http://nkg.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cku.hysaishi.cn

[Q84] 去除首尾空格
来源：http://nyl.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://hfn.yueranfly.top

[Q85] 数值取整
来源：http://gqm.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fwx.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://ztq.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gco.hammf.cn

[Q87] JSON 字段做条件
来源：http://lpt.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gkx.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://wsc.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lzk.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cly.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://oxu.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jjd.hfpthk.cn

[Q90] 生成序号列
来源：http://kea.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kdf.shangyingyoupin.top

================================================================================
来源：http://uoe.chenlongwang.top

R. Bash 专题
来源：http://wvk.guowangkeji.top

================================================================================
来源：http://gym.pycfn.com

[R01] shebang 与严格模式
来源：http://kly.0kj1m.cn

#!/usr/bin/env bash
来源：http://zmv.hfpthk.cn

set -euo pipefail
来源：http://epc.chenzaomai.com

[R02] 变量赋值与使用
来源：http://ptu.iojbl.cn

name="Tom"; echo "$name"
来源：http://mwo.hnxiangtu.top

[R03] 只读变量
来源：http://qxh.nwbrower.top

readonly PI=3.14
来源：http://qia.tanke756.top

[R04] 位置参数
来源：http://paq.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://com.kuanghao11.cn

[R05] 参数默认值
来源：http://bni.daxiang520.top

name="${1:-default}"
来源：http://lio.jiagoushi.top

[R06] 判断命令是否存在
来源：http://flm.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ckv.fehbvm.com

[R07] if 判断文件
来源：http://hmj.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dhe.feifeiyinyue.top

[R08] 数值比较
来源：http://zbd.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ckp.jlsjyb.cn

[R09] 字符串比较
来源：http://ybc.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rjn.yangfankeji.com

[R10] 正则匹配
来源：http://ump.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ofp.cucudq.cn

[R11] case 多分支
来源：http://dbq.zhijiandao.cn

case "$1" in
来源：http://dgm.hesvh.cn

start) echo "启动" ;;
来源：http://yui.daxiang520.top

stop)  echo "停止" ;;
来源：http://bbv.yj20258.top

*)     echo "未知命令" ;;
来源：http://ktk.zhoulong.xyz

esac
来源：http://nix.xinyue.icu

[R12] for 遍历文件
来源：http://xct.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://zuw.hnxiangtu.top

[R13] for 计数循环
来源：http://jzq.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://vaz.zycfv.cn

[R14] C 风格 for
来源：http://qya.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lnv.hywenlv.cn

[R15] while 逐行读文件
来源：http://def.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fhv.gzhubu.top

[R16] until 等待条件
来源：http://xib.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ddy.jlsjyb.cn

[R17] 数组定义与取值
来源：http://nus.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lhu.xuetiantiany.cn

[R18] 遍历数组
来源：http://owq.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wya.fktsv.cn

[R19] 数组长度
来源：http://cvo.9152youxi.cn

echo "${#arr[@]}"
来源：http://pml.ctjpmb.com

[R20] 关联数组（字典）
来源：http://gab.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://byl.ivvv.top

[R21] 字符串长度
来源：http://ltu.yongpay.top

echo "${#s}"
来源：http://lkk.shanyushiyangtech.top

[R22] 截取子串
来源：http://zak.zhongyouzk.top

echo "${s:0:5}"
来源：http://qdm.zhixingplan.top

[R23] 字符串替换
来源：http://iev.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mwz.xylfe.cn

[R24] 大小写转换
来源：http://few.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://dvs.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://pyo.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pnc.haohaochexian.top

[R26] 命令替换
来源：http://syy.meibo888.top

now=$(date +%F); echo "$now"
来源：http://ayh.zhixingplan.top

[R27] 算术展开
来源：http://jib.yongpay.top

echo $((1 + 2 * 3))
来源：http://lws.aizwys.cn

[R28] 浮点运算
来源：http://ohq.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://xqz.svipenyu.cn

[R29] 定义函数
来源：http://jrf.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ogl.316326.xyz

[R30] 函数返回状态码
来源：http://wec.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://clz.zhixingplan.top

[R31] 局部变量
来源：http://cso.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://jnx.hnxiangtu.top

[R32] 参数个数校验
来源：http://lig.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hhi.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://vud.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmu.guowangkeji.top

[R34] 退出时清理
来源：http://xsx.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://fho.cqqwz.cn

[R35] 后台执行并等待
来源：http://zsj.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://atz.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://yyq.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ebq.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://qzi.ybcxt.top

files=$(ls -1)
来源：http://apa.tarul.cn

[R38] 管道串联
来源：http://num.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://gfb.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://wul.yj20258888.top

cmd > out.log 2>&1
来源：http://tqg.sweek.top

[R40] 追加写日志
来源：http://jre.gzhubu.top

echo "log" >> out.log
来源：http://cdt.yj20258888.top

[R41] 丢弃输出
来源：http://yui.316326.xyz

cmd >/dev/null 2>&1
来源：http://cvc.zycfv.cn

[R42] 输入重定向
来源：http://wcz.ctjpmb.com

wc -l < a.txt
来源：http://rhk.gaohongyu789.top

[R43] 按名字查找文件
来源：http://xrm.9152youxi.cn

find . -name "*.log" -type f
来源：http://drt.bjfxy.top

[R44] 按修改时间查找
来源：http://zmh.316326.xyz

find . -mtime -7 -type f
来源：http://vsr.bjfxy.top

[R45] 批量删除
来源：http://hkw.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://prk.yfazqb.com

[R46] 递归替换文件内容
来源：http://kdu.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rhw.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://tha.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dpj.daria6918.cn

[R48] awk 取指定列
来源：http://itk.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://vyp.hongshengwenyu.top

[R49] awk 带条件
来源：http://duq.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zqc.zhongyouzk.top

[R50] awk 求和
来源：http://mfv.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://fcq.fehbvm.com

[R51] 排序去重取前几
来源：http://mfq.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://htu.sufxvd.cn

[R52] 统计行数
来源：http://jrb.zhaomingkeji.xyz

wc -l a.txt
来源：http://oyr.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://mgt.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kqg.hnxiangtu.top

[R54] 比较两个文件
来源：http://yiz.sxryk.cn

diff a.txt b.txt
来源：http://sew.ivvv.top

[R55] 压缩与解压
来源：http://ggg.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mhh.zhengqikj.top

[R56] 远程拷贝
来源：http://xvs.bjfxy.top

scp file user@host:/path/
来源：http://dli.haohaochexian.top

[R57] 远程执行命令
来源：http://hgo.tarul.cn

ssh user@host 'uptime'
来源：http://ekj.aizwys.cn

[R58] 下载文件
来源：http://vxh.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zlg.xziqi.cn

[R59] 发 POST JSON
来源：http://xuc.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rpg.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://ful.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bwa.xinyue.icu

[R61] 磁盘占用
来源：http://igp.nanxuanxn.top

df -h;  du -sh *
来源：http://sul.hesvh.cn

[R62] 找最占空间的文件
来源：http://hek.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://tcu.chenjidiqi.icu

[R63] 内存与进程
来源：http://wjc.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://cvs.xinyue.icu

[R64] 结束进程
来源：http://vxm.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://duc.snrcjt.cn

[R65] 查看端口占用
来源：http://fmu.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vbe.52xcode.cn

[R66] 定时任务
来源：http://kix.jqgufenzy.top

crontab -e;  crontab -l
来源：http://zuq.birdmap.top

[R67] 生成随机十六进制串
来源：http://ndz.shangyingyoupin.top

openssl rand -hex 16
来源：http://wzf.vqdsnc.cn

[R68] 计算文件校验值
来源：http://tvc.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kqs.nanxuanxn.top

[R69] 生成随机密码
来源：http://aqi.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://sbs.ppjwa.cn

[R70] 时间戳与互转
来源：http://arf.tarul.cn

date +%s;  date -d @1700000000
来源：http://mfn.ybcxt.top

[R71] 日期格式化
来源：http://nxg.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://pvk.mhx1999.top

[R72] 等待端口就绪
来源：http://xaw.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://opc.hfpthk.cn

[R73] 分割大日志
来源：http://wwk.hcnkem.com

split -l 1000 big.log part_
来源：http://zii.aibaodan.cn

[R74] 批量重命名
来源：http://wxt.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://utm.shangyingyoupin.top

[R75] 导出环境变量
来源：http://air.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://vsz.ctjpmb.com

[R76] 使用临时文件
来源：http://osw.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yqt.chenjidiqi.icu

[R77] 读取用户输入
来源：http://qen.cdnleiting.top

read -rp "请输入: " ans
来源：http://gas.hammf.cn

[R78] 交互式菜单
来源：http://yrw.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cdo.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://ihp.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wlv.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://vxl.quarkkingdee.top

time ./run.sh
来源：http://zmo.fengsongda.top

================================================================================
来源：http://doy.aizwys.cn

S. C / C++ 专题
来源：http://nmv.iojbl.cn

================================================================================
来源：http://lhx.zhoulong.xyz

[S01] C：Hello World
来源：http://woy.zhiwuduotai.top

#include <stdio.h>
来源：http://mvi.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mfm.aizwys.cn

[S02] C：变量与格式化输出
来源：http://kuv.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://ipy.guowangkeji.top

[S03] C：读入整数
来源：http://klc.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://bol.bbcook.cn

[S04] C：字符串复制
来源：http://enh.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://lhe.cheryme.top

[S05] C：字符串长度
来源：http://tvx.hcnkem.com

strlen(s)
来源：http://dch.hcnkem.com

[S06] C：字符串比较
来源：http://byr.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://oat.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://ckb.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://atg.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://owj.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://noe.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://xxs.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evg.bjfxy.top

[S10] C：指针与解引用
来源：http://oam.redwolf501.top

int *p = &a;  *p = 5;
来源：http://gdt.svipenyu.cn

[S11] C：逐行读文件
来源：http://bxn.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://aff.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxm.nanxuanxn.top

fclose(f);
来源：http://egc.aibaodan.cn

[S12] C：写文件
来源：http://are.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tvt.ybcxt.top

[S13] C：宏定义
来源：http://eob.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jqs.ywan-chungtsiang.top

[S14] C：枚举
来源：http://vgr.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ods.bjfxy.top

[S15] C：类型转换
来源：http://oqk.yonumen.top

(double) a / b
来源：http://uov.guowangkeji.top

[S16] C：位操作置位
来源：http://tmh.hnqzz.top

x |= (1 << 3);
来源：http://pvh.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://eex.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffy.xuetiantiany.cn

[S18] C：命令行参数
来源：http://ohy.fengsongda.top

int main(int argc, char **argv)
来源：http://fhh.feifeiyinyue.top

[S19] C：快速排序
来源：http://pog.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://ecw.sufxvd.cn

[S20] C：二分查找
来源：http://ppd.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aqk.bbcook.cn

[S21] C：字符类别判断
来源：http://cdx.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rrs.xinyue.icu

[S22] C：字符串转数字
来源：http://usb.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://nms.hongshengwenyu.top

[S23] C：随机数
来源：http://iqw.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hqw.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://lcy.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rex.jianghu66.top

[S25] C：内存拷贝
来源：http://yra.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://wfb.epnwcf.com

[S26] C：内存清零
来源：http://abg.gzhubu.top

memset(a, 0, sizeof a);
来源：http://muv.dashuyun.cn

[S27] C：定义常量
来源：http://dhw.andypj.xyz

const double PI = 3.14159;
来源：http://icx.0kj1m.cn

[S28] C：静态变量
来源：http://spk.9152youxi.cn

static int counter = 0;
来源：http://dqv.yangfankeji.com

[S29] C：变参函数
来源：http://iif.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://chu.bjfxy.top

[S30] C：头文件保护
来源：http://xsy.meibo888.top

#ifndef X_H
来源：http://ykr.9152youxi.cn

#define X_H
来源：http://xzs.zdbjq.cn

#endif
来源：http://zam.ppjwa.cn

[S31] C++：Hello World
来源：http://zyq.zhongyouzk.top

#include <iostream>
来源：http://coi.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://baf.wangdashe.top

[S32] C++：字符串
来源：http://gdb.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://xcb.hammf.cn

[S33] C++：vector 增删
来源：http://xnt.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qch.aizwys.cn

[S34] C++：遍历 vector
来源：http://tge.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://fos.chenlongwang.top

[S35] C++：map
来源：http://acb.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfv.haohaochexian.top

[S36] C++：unordered_map
来源：http://sgn.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jas.redwolf501.top

[S37] C++：set
来源：http://gra.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxl.svipenyu.cn

[S38] C++：排序
来源：http://ksn.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://cip.uphjek.com

[S39] C++：自定义比较器排序
来源：http://kgc.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ohe.ehwqpu.com

[S40] C++：查找元素
来源：http://xcj.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zcj.yfazqb.com

[S41] C++：类与构造函数
来源：http://vxk.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vyn.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://eby.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://zvc.hongshengwenyu.top

[S43] C++：智能指针
来源：http://vej.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://rpz.redwolf501.top

[S44] C++：引用传参
来源：http://aab.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://emg.wangdashe.top

[S45] C++：lambda
来源：http://eek.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vku.hongshengwenyu.top

[S46] C++：函数模板
来源：http://eff.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nzm.fzhhl.top


<!-- 参考信息 -->