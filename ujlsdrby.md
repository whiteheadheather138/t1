代发 wailian999

[Q61] 移动平均
来源：http://kym.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cat.9152youxi.cn

[Q62] 分组占比
来源：http://qrr.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mcz.9152youxi.cn

[Q63] 开启事务
来源：http://pyn.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gbh.0kj1m.cn

[Q64] 提交事务
来源：http://uwk.gotoacloud.top

COMMIT;
来源：http://zfx.wangshuangyany.cn

[Q65] 回滚事务
来源：http://qom.nwbrower.top

ROLLBACK;
来源：http://kvt.yj20258888.top

[Q66] 行锁查询
来源：http://fdo.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eac.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://tgs.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xve.sweek.top

[Q68] 保存点
来源：http://jzb.gaohongyu789.top

SAVEPOINT sp1;
来源：http://dts.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://qtd.hesvh.cn

[Q69] 查看执行计划
来源：http://rmg.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qmz.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://oei.yuanzhike.top

ANALYZE TABLE users;
来源：http://vkf.ctjpmb.com

[Q71] 查看建表语句
来源：http://cjf.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dse.dashuyun.cn

[Q72] 查看索引
来源：http://npi.shuidangran.top

SHOW INDEX FROM users;
来源：http://mos.hongshengwenyu.top

[Q73] 查看表状态
来源：http://ife.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fes.havefunace.top

[Q74] 强制使用索引
来源：http://ucq.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xpu.hnxiangtu.top

[Q75] 日期格式化
来源：http://eki.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://avs.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://roa.zhongyouzk.top

[Q76] 按天统计
来源：http://qpy.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qut.epnwcf.com

[Q77] 时间加减
来源：http://oqs.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aql.zhixingplan.top

[Q78] 当前时间
来源：http://kqq.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gpc.ydjk.org.cn

[Q79] 字符串拼接
来源：http://xjx.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fjc.zhoulong.xyz

[Q80] 字符串截取
来源：http://fkc.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://olq.dianchejie.cn

[Q81] 字符串替换
来源：http://fsh.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ptd.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://wlh.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oiv.hongshengwenyu.top

[Q83] 大小写转换
来源：http://ebk.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ibn.jiagoushi.top

[Q84] 去除首尾空格
来源：http://xvo.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://qrk.zhijiandao.cn

[Q85] 数值取整
来源：http://mqx.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rqm.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://jtl.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://efm.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://jbw.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ycl.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://ohb.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://otq.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fav.tianlin.xyz

[Q89] 判断表是否存在
来源：http://brz.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rtb.jinqigufen.top

[Q90] 生成序号列
来源：http://wnt.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yuc.yangfankeji.com

================================================================================
来源：http://fkz.tianlin.xyz

R. Bash 专题
来源：http://xic.wangdashe.top

================================================================================
来源：http://zas.c1oappe.top

[R01] shebang 与严格模式
来源：http://liv.yvedp.cn

#!/usr/bin/env bash
来源：http://fqv.iojbl.cn

set -euo pipefail
来源：http://cpw.hfpthk.cn

[R02] 变量赋值与使用
来源：http://jud.bjfxy.top

name="Tom"; echo "$name"
来源：http://kmp.dashuyun.cn

[R03] 只读变量
来源：http://aty.shuidangran.top

readonly PI=3.14
来源：http://qpr.wangshuangyany.cn

[R04] 位置参数
来源：http://dwd.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fos.zhengqikj.top

[R05] 参数默认值
来源：http://itg.shanyushiyangkeji.top

name="${1:-default}"
来源：http://izh.yonumen.top

[R06] 判断命令是否存在
来源：http://sxc.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kwi.uphjek.com

[R07] if 判断文件
来源：http://qaa.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jny.tarul.cn

[R08] 数值比较
来源：http://zvr.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xjb.shanyushiyangtech.top

[R09] 字符串比较
来源：http://tmc.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://erf.hnqzz.top

[R10] 正则匹配
来源：http://ubk.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eli.jinyuanbaomall.cn

[R11] case 多分支
来源：http://zjd.nwbrower.top

case "$1" in
来源：http://sph.c1oappe.top

start) echo "启动" ;;
来源：http://cjb.ivvv.top

stop)  echo "停止" ;;
来源：http://shl.nwbrower.top

*)     echo "未知命令" ;;
来源：http://cir.zhaomingkeji.xyz

esac
来源：http://arg.nanxuanxn.top

[R12] for 遍历文件
来源：http://gik.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://tgh.pengpengdd.cyou

[R13] for 计数循环
来源：http://qrf.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://ehv.hnqzz.top

[R14] C 风格 for
来源：http://pxy.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dwd.fehbvm.com

[R15] while 逐行读文件
来源：http://eyx.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bju.jqgfzy.top

[R16] until 等待条件
来源：http://xyh.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iia.daxiang520.top

[R17] 数组定义与取值
来源：http://anp.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://iuk.zdbjq.cn

[R18] 遍历数组
来源：http://hjt.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mqf.vqdsnc.cn

[R19] 数组长度
来源：http://ttn.hcnkem.com

echo "${#arr[@]}"
来源：http://uqo.fktsv.cn

[R20] 关联数组（字典）
来源：http://tjq.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cbj.uphjek.com

[R21] 字符串长度
来源：http://qtq.guowangkeji.top

echo "${#s}"
来源：http://bnq.daxiang520.top

[R22] 截取子串
来源：http://rur.pengpengdd.cyou

echo "${s:0:5}"
来源：http://bjf.zhoulong.xyz

[R23] 字符串替换
来源：http://hzi.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndc.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://xqv.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://beu.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://wzq.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uzt.sysykeji.top

[R26] 命令替换
来源：http://kmc.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://mpo.wangshuangyany.cn

[R27] 算术展开
来源：http://qql.fzhhl.top

echo $((1 + 2 * 3))
来源：http://dcy.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://nak.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://omg.xylfe.cn

[R29] 定义函数
来源：http://vmz.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gnu.yj20258.top

[R30] 函数返回状态码
来源：http://pts.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://gjm.fktsv.cn

[R31] 局部变量
来源：http://jcj.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://ymd.shuidangran.top

[R32] 参数个数校验
来源：http://ewv.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://azj.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://wuj.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wow.tarul.cn

[R34] 退出时清理
来源：http://wrc.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://bnc.hesvh.cn

[R35] 后台执行并等待
来源：http://itp.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zfs.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://wts.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tai.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://umx.jlsjyb.cn

files=$(ls -1)
来源：http://zei.sufxvd.cn

[R38] 管道串联
来源：http://sky.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://dzi.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://egy.yj202588.top

cmd > out.log 2>&1
来源：http://xfl.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://kmx.iojbl.cn

echo "log" >> out.log
来源：http://mbe.aibaodan.cn

[R41] 丢弃输出
来源：http://iue.gzhubu.top

cmd >/dev/null 2>&1
来源：http://gct.hfpthk.cn

[R42] 输入重定向
来源：http://azt.dashuyun.cn

wc -l < a.txt
来源：http://uet.xuanzx.com

[R43] 按名字查找文件
来源：http://bpn.cashguo.top

find . -name "*.log" -type f
来源：http://uce.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://vii.jiagoushi.top

find . -mtime -7 -type f
来源：http://vqq.c1oappe.top

[R45] 批量删除
来源：http://agh.cheryme.top

find . -name "*.tmp" -delete
来源：http://thc.yuxming.cn

[R46] 递归替换文件内容
来源：http://hys.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jqx.gaohongyu789.top

[R47] sed 单行替换
来源：http://ger.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://inh.xuetiantiany.cn

[R48] awk 取指定列
来源：http://iqm.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://tjw.cashguo.top

[R49] awk 带条件
来源：http://adq.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zox.zdbjq.cn

[R50] awk 求和
来源：http://uug.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://aku.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://nsh.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rav.shangyingyoupin.top

[R52] 统计行数
来源：http://tgs.chenzaomai.com

wc -l a.txt
来源：http://yhy.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://gvv.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mtd.daria6918.cn

[R54] 比较两个文件
来源：http://gqh.hcnkem.com

diff a.txt b.txt
来源：http://xgx.wangshuangyany.cn

[R55] 压缩与解压
来源：http://kpr.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cde.zdbjq.cn

[R56] 远程拷贝
来源：http://uxw.zhixingplan.top

scp file user@host:/path/
来源：http://mjs.ybcxt.top

[R57] 远程执行命令
来源：http://vwb.yj20258888.top

ssh user@host 'uptime'
来源：http://zpf.cheryme.top

[R58] 下载文件
来源：http://ehq.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nmv.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://dsa.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jic.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://rls.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kpj.daxiang520.top

[R61] 磁盘占用
来源：http://jdh.ehwqpu.com

df -h;  du -sh *
来源：http://izo.pycfn.com

[R62] 找最占空间的文件
来源：http://pka.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://wis.shuidangran.top

[R63] 内存与进程
来源：http://qet.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://enr.hammf.cn

[R64] 结束进程
来源：http://fww.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://ejn.guowangkeji.top

[R65] 查看端口占用
来源：http://qcl.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fdf.vehdjk.com

[R66] 定时任务
来源：http://dmm.zycfv.cn

crontab -e;  crontab -l
来源：http://odd.tanke756.top

[R67] 生成随机十六进制串
来源：http://hfy.fzhhl.top

openssl rand -hex 16
来源：http://qya.ydzc1.top

[R68] 计算文件校验值
来源：http://qvt.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://tze.wangdashe.top

[R69] 生成随机密码
来源：http://spw.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://yay.dashuyun.cn

[R70] 时间戳与互转
来源：http://dua.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://mle.gaohongyu789.top

[R71] 日期格式化
来源：http://anl.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lzb.shuidangran.top

[R72] 等待端口就绪
来源：http://lbu.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wms.chenzaomai.com

[R73] 分割大日志
来源：http://awt.zdqjudy.top

split -l 1000 big.log part_
来源：http://lyg.jinqigfzy.top

[R74] 批量重命名
来源：http://qsd.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hdy.nanxuanxn.top

[R75] 导出环境变量
来源：http://rkq.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://qsz.ppjwa.cn

[R76] 使用临时文件
来源：http://vgr.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bdx.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://qlf.cqqwz.cn

read -rp "请输入: " ans
来源：http://ztc.pengpengdd.cyou

[R78] 交互式菜单
来源：http://qey.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ktn.yuanzhike.top

[R79] 解析命令行选项
来源：http://qwr.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xhr.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://ktk.yj20258.top

time ./run.sh
来源：http://ejz.ppjwa.cn

================================================================================
来源：http://zgg.jyoumei.cn

S. C / C++ 专题
来源：http://xou.dianchejie.cn

================================================================================
来源：http://okt.chenjidiqi.icu

[S01] C：Hello World
来源：http://qcz.ydzc1.top

#include <stdio.h>
来源：http://vww.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yec.epnwcf.com

[S02] C：变量与格式化输出
来源：http://upv.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://jzk.jinqigfzy.top

[S03] C：读入整数
来源：http://cvk.0kj1m.cn

int x; scanf("%d", &x);
来源：http://jai.sweek.top

[S04] C：字符串复制
来源：http://dhc.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://xun.tianlin.xyz

[S05] C：字符串长度
来源：http://gps.daxiang520.top

strlen(s)
来源：http://bot.chenzaomai.com

[S06] C：字符串比较
来源：http://rpd.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://qye.yonumen.top

[S07] C：数组遍历求和
来源：http://nmh.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fli.meibo888.top

[S08] C：动态内存分配与释放
来源：http://lgd.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ock.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://fqy.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://abh.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://xgd.daxiang520.top

int *p = &a;  *p = 5;
来源：http://lwa.smart0.xyz

[S11] C：逐行读文件
来源：http://wwa.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://ogn.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://zgz.gzhubu.top

fclose(f);
来源：http://ajg.aibaodan.cn

[S12] C：写文件
来源：http://oxo.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jyn.hongshengwenyu.top

[S13] C：宏定义
来源：http://mve.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ely.jinghuilouyu.cn

[S14] C：枚举
来源：http://ebt.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://orp.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://eog.yuanzhike.top

(double) a / b
来源：http://ftm.redwolf501.top

[S16] C：位操作置位
来源：http://xwp.52xcode.cn

x |= (1 << 3);
来源：http://ipz.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://hjk.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kuf.jqgfzy.top

[S18] C：命令行参数
来源：http://rrc.sxryk.cn

int main(int argc, char **argv)
来源：http://asv.gaohongyu789.top

[S19] C：快速排序
来源：http://qgu.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jme.tanke756.top

[S20] C：二分查找
来源：http://vpy.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fha.hywenlv.cn

[S21] C：字符类别判断
来源：http://wnv.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kjw.aizwys.cn

[S22] C：字符串转数字
来源：http://aoi.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ehf.nwbrower.top

[S23] C：随机数
来源：http://woc.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://aww.bjfxy.top

[S24] C：获取本地时间
来源：http://erb.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wfr.yfazqb.com

[S25] C：内存拷贝
来源：http://jcj.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://wnj.guannengcc.top

[S26] C：内存清零
来源：http://wky.ydzc1.top

memset(a, 0, sizeof a);
来源：http://bkv.feifeiyinyue.top

[S27] C：定义常量
来源：http://drp.sufxvd.cn

const double PI = 3.14159;
来源：http://kgt.cqqwz.cn

[S28] C：静态变量
来源：http://hgx.yvedp.cn

static int counter = 0;
来源：http://puq.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://gpf.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://san.ehwqpu.com

[S30] C：头文件保护
来源：http://qol.pengpengdd.cyou

#ifndef X_H
来源：http://oxj.yanxiufei.cn

#define X_H
来源：http://nfz.chenlongwang.top

#endif
来源：http://mzy.fzhhl.top

[S31] C++：Hello World
来源：http://bpq.tianlin.xyz


<!-- 参考信息 -->