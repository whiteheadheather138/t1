代发 wailian999

SHOW INDEX FROM users;
来源：http://tvh.hnqzz.top

[Q73] 查看表状态
来源：http://fuk.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aly.hysaishi.cn

[Q74] 强制使用索引
来源：http://nbc.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xve.yangfankeji.com

[Q75] 日期格式化
来源：http://gus.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ywb.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yya.yonumen.top

[Q76] 按天统计
来源：http://oge.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://evy.jinqigfzy.top

[Q77] 时间加减
来源：http://afe.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhx.hysaishi.cn

[Q78] 当前时间
来源：http://xul.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://agv.jqgfzy.top

[Q79] 字符串拼接
来源：http://izn.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zzs.dashuyun.cn

[Q80] 字符串截取
来源：http://ijv.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lci.316326.xyz

[Q81] 字符串替换
来源：http://hgv.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nob.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://fih.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://otb.ehwqpu.com

[Q83] 大小写转换
来源：http://spj.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sll.smart0.xyz

[Q84] 去除首尾空格
来源：http://jct.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://cpu.nanxuanxn.top

[Q85] 数值取整
来源：http://sdg.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cmw.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://lzy.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://drx.yj202588.top

[Q87] JSON 字段做条件
来源：http://dab.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fqq.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://rkx.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sdp.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ezf.tianlin.xyz

[Q89] 判断表是否存在
来源：http://wyq.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcz.vqdsnc.cn

[Q90] 生成序号列
来源：http://xmy.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufb.yangfankeji.com

================================================================================
来源：http://swx.gogol.net.cn

R. Bash 专题
来源：http://mnr.zhengqikj.top

================================================================================
来源：http://uhd.nanxinkj.top

[R01] shebang 与严格模式
来源：http://tzm.hnxiangtu.top

#!/usr/bin/env bash
来源：http://crj.cdnleiting.top

set -euo pipefail
来源：http://fvv.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://pes.ehwqpu.com

name="Tom"; echo "$name"
来源：http://gaf.yuxming.cn

[R03] 只读变量
来源：http://dpt.fanxiaobao.xyz

readonly PI=3.14
来源：http://xia.cheryme.top

[R04] 位置参数
来源：http://lhr.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bms.jqgfzy.top

[R05] 参数默认值
来源：http://oca.9152youxi.cn

name="${1:-default}"
来源：http://zji.fzhhl.top

[R06] 判断命令是否存在
来源：http://qxg.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tcl.hysaishi.cn

[R07] if 判断文件
来源：http://kya.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rep.guannengcc.top

[R08] 数值比较
来源：http://lue.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cha.jqgfzy.top

[R09] 字符串比较
来源：http://jlu.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pui.yueranfly.top

[R10] 正则匹配
来源：http://oqt.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zky.shanyushiyangtech.top

[R11] case 多分支
来源：http://mny.dashuyun.cn

case "$1" in
来源：http://tqh.havefunace.top

start) echo "启动" ;;
来源：http://qsh.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://hhq.pycfn.com

*)     echo "未知命令" ;;
来源：http://cqt.nanxuanxn.top

esac
来源：http://qid.tarul.cn

[R12] for 遍历文件
来源：http://glr.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://oke.gogol.net.cn

[R13] for 计数循环
来源：http://smw.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://mqi.ybcxt.top

[R14] C 风格 for
来源：http://hpg.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ksk.hywenlv.cn

[R15] while 逐行读文件
来源：http://ihg.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mmu.jiagoushi.top

[R16] until 等待条件
来源：http://xso.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://isf.ppjwa.cn

[R17] 数组定义与取值
来源：http://ufl.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gje.fanxiaobao.xyz

[R18] 遍历数组
来源：http://cgm.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qkk.hysaishi.cn

[R19] 数组长度
来源：http://own.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://gec.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://xqr.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfd.sysykeji.top

[R21] 字符串长度
来源：http://usg.bjfxy.top

echo "${#s}"
来源：http://iha.jinyuanbaomall.cn

[R22] 截取子串
来源：http://nfq.jqgufenzy.top

echo "${s:0:5}"
来源：http://rju.fehbvm.com

[R23] 字符串替换
来源：http://suh.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eiy.316326.xyz

[R24] 大小写转换
来源：http://biy.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://prp.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://bjn.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bmz.chenzaomai.com

[R26] 命令替换
来源：http://kiu.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://ikm.shuidangran.top

[R27] 算术展开
来源：http://zfq.andypj.xyz

echo $((1 + 2 * 3))
来源：http://ndx.jqgufenzy.top

[R28] 浮点运算
来源：http://lru.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://zcr.xinyue.icu

[R29] 定义函数
来源：http://hsy.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jdf.ydjk.org.cn

[R30] 函数返回状态码
来源：http://myk.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://ljb.tian-w.cn

[R31] 局部变量
来源：http://fqt.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://ytq.zhongyouzk.top

[R32] 参数个数校验
来源：http://crc.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zgb.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://vth.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zwy.gzhubu.top

[R34] 退出时清理
来源：http://mls.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://cdo.zhixingplan.top

[R35] 后台执行并等待
来源：http://maw.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vbe.0kj1m.cn

[R36] 并发执行多个任务
来源：http://wmy.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zgo.jyoumei.cn

[R37] 把输出赋给变量
来源：http://gfg.xziqi.cn

files=$(ls -1)
来源：http://box.hysaishi.cn

[R38] 管道串联
来源：http://vqz.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://tmz.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://scv.iojbl.cn

cmd > out.log 2>&1
来源：http://uka.bbcook.cn

[R40] 追加写日志
来源：http://mdw.nwbrower.top

echo "log" >> out.log
来源：http://kzi.xuanzx.com

[R41] 丢弃输出
来源：http://fbk.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://axu.52xcode.cn

[R42] 输入重定向
来源：http://iri.guannengcc.top

wc -l < a.txt
来源：http://nje.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://xoq.bbcook.cn

find . -name "*.log" -type f
来源：http://bmp.yangfankeji.com

[R44] 按修改时间查找
来源：http://qkb.fzhhl.top

find . -mtime -7 -type f
来源：http://kwl.52xcode.cn

[R45] 批量删除
来源：http://jnc.hnqzz.top

find . -name "*.tmp" -delete
来源：http://add.svipenyu.cn

[R46] 递归替换文件内容
来源：http://nvi.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lte.zhengqikj.top

[R47] sed 单行替换
来源：http://ixa.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://szp.shuidangran.top

[R48] awk 取指定列
来源：http://zwn.sweek.top

awk '{print $1, $3}' a.txt
来源：http://oam.vehdjk.com

[R49] awk 带条件
来源：http://chn.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yoa.shzxlz.cn

[R50] awk 求和
来源：http://zcw.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://svo.316326.xyz

[R51] 排序去重取前几
来源：http://gsq.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://jgz.zhixingplan.top

[R52] 统计行数
来源：http://nbs.hnxiangtu.top

wc -l a.txt
来源：http://itf.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://nbv.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vbv.52xcode.cn

[R54] 比较两个文件
来源：http://esy.yvedp.cn

diff a.txt b.txt
来源：http://mvb.yj20258888.top

[R55] 压缩与解压
来源：http://kdt.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://shb.iojbl.cn

[R56] 远程拷贝
来源：http://zop.ybcxt.top

scp file user@host:/path/
来源：http://ndy.cucudq.cn

[R57] 远程执行命令
来源：http://ete.bbcook.cn

ssh user@host 'uptime'
来源：http://dyq.jinyuanbaomall.cn

[R58] 下载文件
来源：http://cei.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mfj.zhongyouzk.top

[R59] 发 POST JSON
来源：http://eyd.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ont.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://brj.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ujr.sufxvd.cn

[R61] 磁盘占用
来源：http://swk.mhx1999.top

df -h;  du -sh *
来源：http://srh.jinqigufen.top

[R62] 找最占空间的文件
来源：http://ovy.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://ezl.0kj1m.cn

[R63] 内存与进程
来源：http://dux.cheryme.top

free -h;  ps aux | grep nginx
来源：http://ksu.zhoulong.xyz

[R64] 结束进程
来源：http://rsy.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://lup.ctjpmb.com

[R65] 查看端口占用
来源：http://ndu.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fkd.svipenyu.cn

[R66] 定时任务
来源：http://jtl.hywenlv.cn

crontab -e;  crontab -l
来源：http://iue.xylfe.cn

[R67] 生成随机十六进制串
来源：http://piy.hongshengwenyu.top

openssl rand -hex 16
来源：http://poo.meibo888.top

[R68] 计算文件校验值
来源：http://uxy.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xhd.iojbl.cn

[R69] 生成随机密码
来源：http://gac.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://cdk.vehdjk.com

[R70] 时间戳与互转
来源：http://bla.yj20258.top

date +%s;  date -d @1700000000
来源：http://ajo.sjlbkw.cn

[R71] 日期格式化
来源：http://uil.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hcq.gogol.net.cn

[R72] 等待端口就绪
来源：http://pva.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mkx.ctjpmb.com

[R73] 分割大日志
来源：http://kfr.52xcode.cn

split -l 1000 big.log part_
来源：http://xyc.ctjpmb.com

[R74] 批量重命名
来源：http://cgm.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tqg.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://ymz.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://idc.quarkkingdee.top

[R76] 使用临时文件
来源：http://eqg.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xsp.aibaodan.cn

[R77] 读取用户输入
来源：http://uqi.jiagoushi.top

read -rp "请输入: " ans
来源：http://xme.hywenlv.cn

[R78] 交互式菜单
来源：http://enc.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://blc.birdmap.top

[R79] 解析命令行选项
来源：http://nuy.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ugf.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://jbb.jlsjyb.cn

time ./run.sh
来源：http://wen.chenjidiqi.icu

================================================================================
来源：http://lrf.chenzaomai.com

S. C / C++ 专题
来源：http://jqo.snrcjt.cn

================================================================================
来源：http://vdf.fanxiaobao.xyz

[S01] C：Hello World
来源：http://dtq.meibo888.top

#include <stdio.h>
来源：http://sby.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://spn.uphjek.com

[S02] C：变量与格式化输出
来源：http://jmd.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://ncy.xziqi.cn

[S03] C：读入整数
来源：http://pwg.yueranfly.top

int x; scanf("%d", &x);
来源：http://mku.gaohongyu789.top

[S04] C：字符串复制
来源：http://pxh.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ppv.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://uun.jlsjyb.cn

strlen(s)
来源：http://khs.jlsjyb.cn

[S06] C：字符串比较
来源：http://svy.cucudq.cn

strcmp(a, b) == 0
来源：http://aad.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://vtz.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xqo.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://sql.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wel.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://vnu.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jvs.zdqjudy.top

[S10] C：指针与解引用
来源：http://jkl.yueranfly.top

int *p = &a;  *p = 5;
来源：http://eap.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://you.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://tta.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nfj.jqgufenzy.top

fclose(f);
来源：http://pbl.havefunace.top

[S12] C：写文件
来源：http://wvy.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ijw.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://imw.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cfx.vqdsnc.cn

[S14] C：枚举
来源：http://izq.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://mka.iojbl.cn

[S15] C：类型转换
来源：http://vsf.zhengqikj.top

(double) a / b
来源：http://tku.yueranfly.top

[S16] C：位操作置位
来源：http://qbb.sysykeji.top

x |= (1 << 3);
来源：http://jkb.pycfn.com

[S17] C：安全拼接字符串
来源：http://pmx.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzg.tian-w.cn

[S18] C：命令行参数
来源：http://bol.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://xmp.zhijiandao.cn

[S19] C：快速排序
来源：http://vur.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://dnu.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://yko.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ozr.zycfv.cn

[S21] C：字符类别判断
来源：http://fxs.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ids.redwolf501.top

[S22] C：字符串转数字
来源：http://kpd.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://jxu.yongpay.top

[S23] C：随机数
来源：http://syl.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oqh.yonumen.top

[S24] C：获取本地时间
来源：http://dzs.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hzz.haohaochexian.top

[S25] C：内存拷贝
来源：http://opu.cqqwz.cn

memcpy(dst, src, n);
来源：http://mqp.chenzaomai.com

[S26] C：内存清零
来源：http://pdb.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://zgg.jianghu66.top

[S27] C：定义常量
来源：http://scj.redwolf501.top

const double PI = 3.14159;
来源：http://fdi.redwolf501.top

[S28] C：静态变量
来源：http://wfv.xingfuxueyuan.xyz

static int counter = 0;
来源：http://qbv.hammf.cn

[S29] C：变参函数
来源：http://jph.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ydk.zycfv.cn

[S30] C：头文件保护
来源：http://bdw.shangyingyoupin.top

#ifndef X_H
来源：http://yml.yuxming.cn

#define X_H
来源：http://lxu.316326.xyz

#endif
来源：http://plo.shangyingyoupin.top

[S31] C++：Hello World
来源：http://soo.fehbvm.com

#include <iostream>
来源：http://srs.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://uvj.fzhhl.top

[S32] C++：字符串
来源：http://olr.cashguo.top

std::string s = "hi";  s += "!";
来源：http://msr.haohaochexian.top

[S33] C++：vector 增删
来源：http://owu.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dwu.fehbvm.com

[S34] C++：遍历 vector
来源：http://cak.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://lkx.zdqjudy.top

[S35] C++：map
来源：http://sdv.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zgg.shuidangran.top

[S36] C++：unordered_map
来源：http://ksx.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eik.birdmap.top

[S37] C++：set
来源：http://yff.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://erg.jqgfzy.top

[S38] C++：排序
来源：http://rxk.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://ojp.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://pqs.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://joa.fktsv.cn

[S40] C++：查找元素
来源：http://qwm.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mte.cashguo.top

[S41] C++：类与构造函数
来源：http://feb.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dmv.andypj.xyz

[S42] C++：继承与虚函数
来源：http://lqc.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://rnb.yueranfly.top


<!-- 参考信息 -->