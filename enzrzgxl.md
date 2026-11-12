代发 wailian999

SHOW INDEX FROM users;
来源：http://ghd.pycfn.com

[Q73] 查看表状态
来源：http://ocl.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://brr.sufxvd.cn

[Q74] 强制使用索引
来源：http://ays.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tph.kuanghao11.cn

[Q75] 日期格式化
来源：http://tgl.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tbr.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qle.zhiwuduotai.top

[Q76] 按天统计
来源：http://hno.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qjb.vqdsnc.cn

[Q77] 时间加减
来源：http://sye.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gvt.xuetiantiany.cn

[Q78] 当前时间
来源：http://tao.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tdf.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://spx.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nie.bbcook.cn

[Q80] 字符串截取
来源：http://yum.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nxw.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://xla.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pfm.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://oaz.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jsi.zhixingplan.top

[Q83] 大小写转换
来源：http://hbv.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hmi.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://bml.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://bhm.jinqigufen.top

[Q85] 数值取整
来源：http://rxq.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mtc.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://xmg.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://arx.pycfn.com

[Q87] JSON 字段做条件
来源：http://osm.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jdf.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://mek.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sug.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kaj.iojbl.cn

[Q89] 判断表是否存在
来源：http://ike.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsx.feifeiyinyue.top

[Q90] 生成序号列
来源：http://tzc.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhj.ehwqpu.com

================================================================================
来源：http://uoo.jinyuanbaomall.cn

R. Bash 专题
来源：http://syi.tian-w.cn

================================================================================
来源：http://nnh.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://fwg.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://mjn.yuanzhike.top

set -euo pipefail
来源：http://yqj.zhengqikj.top

[R02] 变量赋值与使用
来源：http://dsj.zhixingplan.top

name="Tom"; echo "$name"
来源：http://vmg.yangfankeji.com

[R03] 只读变量
来源：http://qqo.uphjek.com

readonly PI=3.14
来源：http://psa.nanxinkj.top

[R04] 位置参数
来源：http://eko.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fbi.cdnleiting.top

[R05] 参数默认值
来源：http://mbz.yj20258888.top

name="${1:-default}"
来源：http://dss.jiagoushi.top

[R06] 判断命令是否存在
来源：http://bhx.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifg.nanxuanxn.top

[R07] if 判断文件
来源：http://ray.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bwi.andypj.xyz

[R08] 数值比较
来源：http://daj.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sng.gzhubu.top

[R09] 字符串比较
来源：http://qbq.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mil.iojbl.cn

[R10] 正则匹配
来源：http://xxs.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ixk.ehwqpu.com

[R11] case 多分支
来源：http://lvl.birdmap.top

case "$1" in
来源：http://shw.jlsjyb.cn

start) echo "启动" ;;
来源：http://rje.wangdashe.top

stop)  echo "停止" ;;
来源：http://irs.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://eal.jyoumei.cn

esac
来源：http://aad.vehdjk.com

[R12] for 遍历文件
来源：http://hxq.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://cpv.jianghu66.top

[R13] for 计数循环
来源：http://ays.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://llq.jianghu66.top

[R14] C 风格 for
来源：http://myg.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dkw.xylfe.cn

[R15] while 逐行读文件
来源：http://fif.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ghh.ivvv.top

[R16] until 等待条件
来源：http://wbk.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zhu.yongpay.top

[R17] 数组定义与取值
来源：http://jyj.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://clt.redwolf501.top

[R18] 遍历数组
来源：http://qge.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hds.guannengcc.top

[R19] 数组长度
来源：http://fhz.shzxlz.cn

echo "${#arr[@]}"
来源：http://iym.zycfv.cn

[R20] 关联数组（字典）
来源：http://fiy.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fwm.tian-w.cn

[R21] 字符串长度
来源：http://zxp.bbcook.cn

echo "${#s}"
来源：http://efe.ydzc1.top

[R22] 截取子串
来源：http://vws.cashguo.top

echo "${s:0:5}"
来源：http://dbt.birdmap.top

[R23] 字符串替换
来源：http://ktr.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vqa.0kj1m.cn

[R24] 大小写转换
来源：http://bwr.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://onb.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://orh.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://drz.nanxuanxn.top

[R26] 命令替换
来源：http://ksc.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://woe.sjlbkw.cn

[R27] 算术展开
来源：http://pqz.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://yvj.epnwcf.com

[R28] 浮点运算
来源：http://qfk.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://ulo.yj202588.top

[R29] 定义函数
来源：http://dud.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jix.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://huc.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://wnm.52xcode.cn

[R31] 局部变量
来源：http://ciq.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://glz.guannengcc.top

[R32] 参数个数校验
来源：http://pog.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vbr.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://rqp.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fke.fktsv.cn

[R34] 退出时清理
来源：http://vgk.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pkc.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://qcb.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tpj.zhengqikj.top

[R36] 并发执行多个任务
来源：http://lhd.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lyb.yueranfly.top

[R37] 把输出赋给变量
来源：http://rbg.zycfv.cn

files=$(ls -1)
来源：http://yrp.birdmap.top

[R38] 管道串联
来源：http://ehs.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://amr.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://chp.c1oappe.top

cmd > out.log 2>&1
来源：http://axs.shzxlz.cn

[R40] 追加写日志
来源：http://xvu.zhengqikj.top

echo "log" >> out.log
来源：http://kye.smart0.xyz

[R41] 丢弃输出
来源：http://wgp.iojbl.cn

cmd >/dev/null 2>&1
来源：http://xqz.ctjpmb.com

[R42] 输入重定向
来源：http://nuh.bjfxy.top

wc -l < a.txt
来源：http://wrd.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://tvw.daria6918.cn

find . -name "*.log" -type f
来源：http://yzz.ehwqpu.com

[R44] 按修改时间查找
来源：http://irx.jinqigfzy.top

find . -mtime -7 -type f
来源：http://kzv.guannengcc.top

[R45] 批量删除
来源：http://usi.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://rfs.gogol.net.cn

[R46] 递归替换文件内容
来源：http://mwa.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://stc.shangyingyoupin.top

[R47] sed 单行替换
来源：http://yvh.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://wji.yonumen.top

[R48] awk 取指定列
来源：http://szx.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://evj.jqgufenzy.top

[R49] awk 带条件
来源：http://yfh.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gkm.aizwys.cn

[R50] awk 求和
来源：http://nnk.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://joe.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://ieg.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ohm.zhixingplan.top

[R52] 统计行数
来源：http://dei.andypj.xyz

wc -l a.txt
来源：http://xpz.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://seb.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fyb.jyoumei.cn

[R54] 比较两个文件
来源：http://tmc.tarul.cn

diff a.txt b.txt
来源：http://pdi.hcnkem.com

[R55] 压缩与解压
来源：http://pqp.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ies.fehbvm.com

[R56] 远程拷贝
来源：http://tsy.cheryme.top

scp file user@host:/path/
来源：http://tax.haohaochexian.top

[R57] 远程执行命令
来源：http://ivg.ctjpmb.com

ssh user@host 'uptime'
来源：http://qww.yanxiufei.cn

[R58] 下载文件
来源：http://hrb.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wco.52xcode.cn

[R59] 发 POST JSON
来源：http://wso.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://woy.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://ytb.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mpg.epnwcf.com

[R61] 磁盘占用
来源：http://pdi.sweek.top

df -h;  du -sh *
来源：http://rlz.nanxinkj.top

[R62] 找最占空间的文件
来源：http://blx.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://wxu.yj20258888.top

[R63] 内存与进程
来源：http://qqu.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://sjr.ydjk.org.cn

[R64] 结束进程
来源：http://ndf.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://vgc.guannengcc.top

[R65] 查看端口占用
来源：http://vmn.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pdd.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://kfh.tarul.cn

crontab -e;  crontab -l
来源：http://dbq.uphjek.com

[R67] 生成随机十六进制串
来源：http://wjt.dashuyun.cn

openssl rand -hex 16
来源：http://fpb.hfpthk.cn

[R68] 计算文件校验值
来源：http://cbi.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://nby.bbcook.cn

[R69] 生成随机密码
来源：http://uup.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://bax.shuidangran.top

[R70] 时间戳与互转
来源：http://esz.hammf.cn

date +%s;  date -d @1700000000
来源：http://leb.vehdjk.com

[R71] 日期格式化
来源：http://lvp.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gho.vqdsnc.cn

[R72] 等待端口就绪
来源：http://ltv.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://spy.cqqwz.cn

[R73] 分割大日志
来源：http://bhf.cashguo.top

split -l 1000 big.log part_
来源：http://pwk.yueranfly.top

[R74] 批量重命名
来源：http://rpp.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vog.hnxiangtu.top

[R75] 导出环境变量
来源：http://vtl.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://hts.yonumen.top

[R76] 使用临时文件
来源：http://hgo.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://itx.hnxiangtu.top

[R77] 读取用户输入
来源：http://jue.sjlbkw.cn

read -rp "请输入: " ans
来源：http://xgv.hysaishi.cn

[R78] 交互式菜单
来源：http://qba.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dae.yangfankeji.com

[R79] 解析命令行选项
来源：http://juj.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uyc.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://bps.zhongyouzk.top

time ./run.sh
来源：http://cku.yvedp.cn

================================================================================
来源：http://sla.xinyue.icu

S. C / C++ 专题
来源：http://cmu.epnwcf.com

================================================================================
来源：http://zea.guannengcc.top

[S01] C：Hello World
来源：http://zvz.yj20258888.top

#include <stdio.h>
来源：http://eck.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lma.ybcxt.top

[S02] C：变量与格式化输出
来源：http://sfm.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://viz.snrcjt.cn

[S03] C：读入整数
来源：http://ruq.redwolf501.top

int x; scanf("%d", &x);
来源：http://vxx.jinqigfzy.top

[S04] C：字符串复制
来源：http://org.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vda.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://jyo.ppjwa.cn

strlen(s)
来源：http://lor.jqgfzy.top

[S06] C：字符串比较
来源：http://efg.cheryme.top

strcmp(a, b) == 0
来源：http://aaw.ehwqpu.com

[S07] C：数组遍历求和
来源：http://uqh.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ulw.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://wrq.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://moo.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://tta.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://esq.chenzaomai.com

[S10] C：指针与解引用
来源：http://xwf.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://wqo.wangdashe.top

[S11] C：逐行读文件
来源：http://dyk.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://dcv.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kxq.nanxinkj.top

fclose(f);
来源：http://rzn.gotoacloud.top

[S12] C：写文件
来源：http://pbn.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uqa.52xcode.cn

[S13] C：宏定义
来源：http://bhj.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oaj.tarul.cn

[S14] C：枚举
来源：http://hkn.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://zvy.kuanghao11.cn

[S15] C：类型转换
来源：http://nja.mhx1999.top

(double) a / b
来源：http://nub.zdbjq.cn

[S16] C：位操作置位
来源：http://xyj.bjfxy.top

x |= (1 << 3);
来源：http://uxa.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://nuc.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ikv.c1oappe.top

[S18] C：命令行参数
来源：http://yqv.havefunace.top

int main(int argc, char **argv)
来源：http://sjk.pycfn.com

[S19] C：快速排序
来源：http://lbt.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://shg.chenjidiqi.icu

[S20] C：二分查找
来源：http://hhx.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nuo.vehdjk.com

[S21] C：字符类别判断
来源：http://mti.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hzr.zhengqikj.top

[S22] C：字符串转数字
来源：http://bzd.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://bzq.xylfe.cn

[S23] C：随机数
来源：http://fyk.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://upf.ehwqpu.com

[S24] C：获取本地时间
来源：http://rne.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mhw.vqdsnc.cn

[S25] C：内存拷贝
来源：http://tzl.nanxinkj.top

memcpy(dst, src, n);
来源：http://ece.316326.xyz

[S26] C：内存清零
来源：http://tiy.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://xan.xuanzx.com

[S27] C：定义常量
来源：http://hbb.zhiwuduotai.top

const double PI = 3.14159;
来源：http://nrf.gaohongyu789.top

[S28] C：静态变量
来源：http://vpl.svipenyu.cn

static int counter = 0;
来源：http://dvr.xuanzx.com

[S29] C：变参函数
来源：http://lek.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://koo.bbcook.cn

[S30] C：头文件保护
来源：http://awg.shzxlz.cn

#ifndef X_H
来源：http://xmq.cashguo.top

#define X_H
来源：http://req.jianghu66.top

#endif
来源：http://rwa.redwolf501.top

[S31] C++：Hello World
来源：http://uqs.birdmap.top

#include <iostream>
来源：http://vne.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://fpw.vqdsnc.cn

[S32] C++：字符串
来源：http://dei.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://yoq.bbcook.cn

[S33] C++：vector 增删
来源：http://lcz.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fcn.vehdjk.com

[S34] C++：遍历 vector
来源：http://zje.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://dhd.ybcxt.top

[S35] C++：map
来源：http://lsz.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oip.yueranfly.top

[S36] C++：unordered_map
来源：http://lpm.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gkg.jinghuilouyu.cn

[S37] C++：set
来源：http://hea.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://law.jinghuilouyu.cn

[S38] C++：排序
来源：http://ldx.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://iqn.tanke756.top

[S39] C++：自定义比较器排序
来源：http://kia.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kgy.jqgfzy.top

[S40] C++：查找元素
来源：http://psz.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dzc.tanke756.top

[S41] C++：类与构造函数
来源：http://wrc.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ywm.yj20258888.top

[S42] C++：继承与虚函数
来源：http://cpk.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://ltz.ydjk.org.cn


<!-- 参考信息 -->