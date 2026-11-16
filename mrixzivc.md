代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rqh.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://xua.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://npc.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rte.cashguo.top

[Q61] 移动平均
来源：http://szq.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mtc.dianchejie.cn

[Q62] 分组占比
来源：http://yqz.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zkv.vehdjk.com

[Q63] 开启事务
来源：http://oad.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://woo.hcnkem.com

[Q64] 提交事务
来源：http://kbs.zhijiandao.cn

COMMIT;
来源：http://wvd.ppjwa.cn

[Q65] 回滚事务
来源：http://ylm.jlsjyb.cn

ROLLBACK;
来源：http://qvt.yueranfly.top

[Q66] 行锁查询
来源：http://uca.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cuj.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://yzy.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gqy.pycfn.com

[Q68] 保存点
来源：http://pas.chenlongwang.top

SAVEPOINT sp1;
来源：http://vfj.ehwqpu.com

ROLLBACK TO sp1;
来源：http://cdl.zhoulong.xyz

[Q69] 查看执行计划
来源：http://dyg.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://reu.yanxiufei.cn

[Q70] 更新统计信息
来源：http://nlk.smart0.xyz

ANALYZE TABLE users;
来源：http://hni.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://vux.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dch.0kj1m.cn

[Q72] 查看索引
来源：http://mfa.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://fkx.xinyue.icu

[Q73] 查看表状态
来源：http://dsu.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://bir.ppjwa.cn

[Q74] 强制使用索引
来源：http://vze.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wvs.andypj.xyz

[Q75] 日期格式化
来源：http://rts.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ftp.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xeq.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://vbv.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eso.gaohongyu789.top

[Q77] 时间加减
来源：http://jji.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cqn.yonumen.top

[Q78] 当前时间
来源：http://orn.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ikk.mhx1999.top

[Q79] 字符串拼接
来源：http://wzu.ehwqpu.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://byf.shzxlz.cn

[Q80] 字符串截取
来源：http://oie.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dcs.chenlongwang.top

[Q81] 字符串替换
来源：http://ggv.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kfs.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://zac.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oda.yuanzhike.top

[Q83] 大小写转换
来源：http://pbn.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wua.cheryme.top

[Q84] 去除首尾空格
来源：http://vcz.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://rnb.ctjpmb.com

[Q85] 数值取整
来源：http://ylz.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lxw.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://hyg.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ogh.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://ira.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pyf.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://pej.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyj.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oqe.ppjwa.cn

[Q89] 判断表是否存在
来源：http://uut.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ewx.jinqigfzy.top

[Q90] 生成序号列
来源：http://ufc.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://grx.zycfv.cn

================================================================================
来源：http://van.tanke756.top

R. Bash 专题
来源：http://gvs.ydjk.org.cn

================================================================================
来源：http://qzs.hywenlv.cn

[R01] shebang 与严格模式
来源：http://iew.birdmap.top

#!/usr/bin/env bash
来源：http://amn.snrcjt.cn

set -euo pipefail
来源：http://eux.yongpay.top

[R02] 变量赋值与使用
来源：http://tdr.c1oappe.top

name="Tom"; echo "$name"
来源：http://aea.zdqjudy.top

[R03] 只读变量
来源：http://spp.vqdsnc.cn

readonly PI=3.14
来源：http://cnz.zhengqikj.top

[R04] 位置参数
来源：http://qcp.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mey.gzhubu.top

[R05] 参数默认值
来源：http://fup.9152youxi.cn

name="${1:-default}"
来源：http://dou.vehdjk.com

[R06] 判断命令是否存在
来源：http://woj.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xok.hesvh.cn

[R07] if 判断文件
来源：http://sex.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://srl.vehdjk.com

[R08] 数值比较
来源：http://afs.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://rya.daria6918.cn

[R09] 字符串比较
来源：http://sct.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kyd.gzhubu.top

[R10] 正则匹配
来源：http://eop.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://val.zhongyouzk.top

[R11] case 多分支
来源：http://lvq.zhoulong.xyz

case "$1" in
来源：http://vrt.nanxuanxn.top

start) echo "启动" ;;
来源：http://gxl.jqgfzy.top

stop)  echo "停止" ;;
来源：http://dqo.ydzc1.top

*)     echo "未知命令" ;;
来源：http://erd.ppjwa.cn

esac
来源：http://iyo.hammf.cn

[R12] for 遍历文件
来源：http://xaj.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://yuf.yuanzhike.top

[R13] for 计数循环
来源：http://bvv.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://hrj.kuanghao11.cn

[R14] C 风格 for
来源：http://bje.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hyt.jlsjyb.cn

[R15] while 逐行读文件
来源：http://bfe.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gvh.ybcxt.top

[R16] until 等待条件
来源：http://utz.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xgr.nanxuanxn.top

[R17] 数组定义与取值
来源：http://fsh.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://tam.zhiwuduotai.top

[R18] 遍历数组
来源：http://lme.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yss.hammf.cn

[R19] 数组长度
来源：http://qfi.daxiang520.top

echo "${#arr[@]}"
来源：http://njp.birdmap.top

[R20] 关联数组（字典）
来源：http://ovd.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bgj.guowangkeji.top

[R21] 字符串长度
来源：http://ykw.haohaochexian.top

echo "${#s}"
来源：http://nnd.sufxvd.cn

[R22] 截取子串
来源：http://ewy.gotoacloud.top

echo "${s:0:5}"
来源：http://xzf.jianghu66.top

[R23] 字符串替换
来源：http://gof.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lqa.wangshuangyany.cn

[R24] 大小写转换
来源：http://dsk.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://zdm.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://erp.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kwr.hongshengwenyu.top

[R26] 命令替换
来源：http://pne.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://kiz.shzxlz.cn

[R27] 算术展开
来源：http://kfk.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://zrv.hywenlv.cn

[R28] 浮点运算
来源：http://czg.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://rdw.ctjpmb.com

[R29] 定义函数
来源：http://yoe.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pfe.wangdashe.top

[R30] 函数返回状态码
来源：http://uic.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://cnv.c1oappe.top

[R31] 局部变量
来源：http://bsl.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://fgx.cdnleiting.top

[R32] 参数个数校验
来源：http://mws.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xhk.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://tse.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tik.yonumen.top

[R34] 退出时清理
来源：http://nma.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qhk.nanxinkj.top

[R35] 后台执行并等待
来源：http://roo.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qlv.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://qwr.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nwo.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://vmk.tanke756.top

files=$(ls -1)
来源：http://slm.fehbvm.com

[R38] 管道串联
来源：http://qdr.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://ygl.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://hsu.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://gnu.kuanghao11.cn

[R40] 追加写日志
来源：http://dwr.xziqi.cn

echo "log" >> out.log
来源：http://xqm.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://abj.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://uef.gzhubu.top

[R42] 输入重定向
来源：http://oye.epnwcf.com

wc -l < a.txt
来源：http://vbh.zycfv.cn

[R43] 按名字查找文件
来源：http://npu.meibo888.top

find . -name "*.log" -type f
来源：http://dcx.daxiang520.top

[R44] 按修改时间查找
来源：http://sfw.yj20258.top

find . -mtime -7 -type f
来源：http://gbh.xuanzx.com

[R45] 批量删除
来源：http://ivd.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://yho.daxiang520.top

[R46] 递归替换文件内容
来源：http://wna.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tse.mhx1999.top

[R47] sed 单行替换
来源：http://xxi.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dmp.yonumen.top

[R48] awk 取指定列
来源：http://yyp.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://jxd.hnxiangtu.top

[R49] awk 带条件
来源：http://krk.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cwr.hnxiangtu.top

[R50] awk 求和
来源：http://ubw.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aux.aibaodan.cn

[R51] 排序去重取前几
来源：http://uty.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vdl.jinghuilouyu.cn

[R52] 统计行数
来源：http://wwo.ydzc1.top

wc -l a.txt
来源：http://euv.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://azm.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whw.tian-w.cn

[R54] 比较两个文件
来源：http://qkn.vqdsnc.cn

diff a.txt b.txt
来源：http://dxr.yanxiufei.cn

[R55] 压缩与解压
来源：http://vlo.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tur.gotoacloud.top

[R56] 远程拷贝
来源：http://toj.tarul.cn

scp file user@host:/path/
来源：http://hvo.daria6918.cn

[R57] 远程执行命令
来源：http://nrc.xuanzx.com

ssh user@host 'uptime'
来源：http://prc.52xcode.cn

[R58] 下载文件
来源：http://eci.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cmc.shuidangran.top

[R59] 发 POST JSON
来源：http://zgx.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hdn.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://bbb.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zwm.wangdashe.top

[R61] 磁盘占用
来源：http://gae.quarkkingdee.top

df -h;  du -sh *
来源：http://wwl.yuxming.cn

[R62] 找最占空间的文件
来源：http://eiq.yongpay.top

du -ah . | sort -rh | head -10
来源：http://vjj.havefunace.top

[R63] 内存与进程
来源：http://bkj.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://waw.zhijiandao.cn

[R64] 结束进程
来源：http://vtm.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://wok.redwolf501.top

[R65] 查看端口占用
来源：http://rie.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pfe.ydzc1.top

[R66] 定时任务
来源：http://oht.uphjek.com

crontab -e;  crontab -l
来源：http://hpy.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://bji.fanxiaobao.xyz

openssl rand -hex 16
来源：http://nae.shuidangran.top

[R68] 计算文件校验值
来源：http://dti.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://fzx.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://fgl.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://kee.cdnleiting.top

[R70] 时间戳与互转
来源：http://dtd.tarul.cn

date +%s;  date -d @1700000000
来源：http://dfc.yueranfly.top

[R71] 日期格式化
来源：http://hec.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uhz.sjlbkw.cn

[R72] 等待端口就绪
来源：http://ckt.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uld.yanxiufei.cn

[R73] 分割大日志
来源：http://tud.epnwcf.com

split -l 1000 big.log part_
来源：http://szu.yonumen.top

[R74] 批量重命名
来源：http://ubq.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://heq.quarkkingdee.top

[R75] 导出环境变量
来源：http://udv.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://sdk.cdnleiting.top

[R76] 使用临时文件
来源：http://wtv.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kyo.daria6918.cn

[R77] 读取用户输入
来源：http://sub.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://alm.ctjpmb.com

[R78] 交互式菜单
来源：http://xtw.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zow.ppjwa.cn

[R79] 解析命令行选项
来源：http://mcq.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://esr.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://lte.cqqwz.cn

time ./run.sh
来源：http://izh.daria6918.cn

================================================================================
来源：http://wie.jqgfzy.top

S. C / C++ 专题
来源：http://ckv.jqgfzy.top

================================================================================
来源：http://cyq.jianghu66.top

[S01] C：Hello World
来源：http://qrq.jqgufenzy.top

#include <stdio.h>
来源：http://egb.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gkl.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://mvk.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://ffj.vehdjk.com

[S03] C：读入整数
来源：http://qsi.0kj1m.cn

int x; scanf("%d", &x);
来源：http://prk.zhoulong.xyz

[S04] C：字符串复制
来源：http://fcz.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://zez.yonumen.top

[S05] C：字符串长度
来源：http://bkr.havefunace.top

strlen(s)
来源：http://cns.nanxinkj.top

[S06] C：字符串比较
来源：http://cti.smart0.xyz

strcmp(a, b) == 0
来源：http://zct.yonumen.top

[S07] C：数组遍历求和
来源：http://djl.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sgr.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://pfl.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dkr.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://fpn.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lfz.chenlongwang.top

[S10] C：指针与解引用
来源：http://xlr.redwolf501.top

int *p = &a;  *p = 5;
来源：http://iaq.cdnleiting.top

[S11] C：逐行读文件
来源：http://oed.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://imf.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://orx.gotoacloud.top

fclose(f);
来源：http://jde.gotoacloud.top

[S12] C：写文件
来源：http://duy.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nvi.ydjk.org.cn

[S13] C：宏定义
来源：http://sku.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lkr.gotoacloud.top

[S14] C：枚举
来源：http://aji.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://acj.yj20258.top

[S15] C：类型转换
来源：http://zuy.xylfe.cn

(double) a / b
来源：http://klt.yvedp.cn

[S16] C：位操作置位
来源：http://hfw.c1oappe.top

x |= (1 << 3);
来源：http://qhi.xinyue.icu

[S17] C：安全拼接字符串
来源：http://lxp.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sds.ctjpmb.com

[S18] C：命令行参数
来源：http://red.yuanzhike.top

int main(int argc, char **argv)
来源：http://ecz.yanxiufei.cn

[S19] C：快速排序
来源：http://tcd.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://jkn.svipenyu.cn

[S20] C：二分查找
来源：http://emf.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ztb.pycfn.com

[S21] C：字符类别判断
来源：http://cde.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qxt.cucudq.cn

[S22] C：字符串转数字
来源：http://omu.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://dee.xylfe.cn

[S23] C：随机数
来源：http://ofc.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kye.sxryk.cn

[S24] C：获取本地时间
来源：http://gaj.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://axl.tarul.cn

[S25] C：内存拷贝
来源：http://fwk.zdbjq.cn

memcpy(dst, src, n);
来源：http://sss.hnqzz.top

[S26] C：内存清零
来源：http://eqt.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://cje.jianghu66.top

[S27] C：定义常量
来源：http://czt.sufxvd.cn

const double PI = 3.14159;
来源：http://kqp.yvedp.cn

[S28] C：静态变量
来源：http://vkf.hnxiangtu.top

static int counter = 0;
来源：http://qzq.iojbl.cn

[S29] C：变参函数
来源：http://kvv.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gbs.xziqi.cn

[S30] C：头文件保护
来源：http://qbk.jianghu66.top


<!-- 参考信息 -->