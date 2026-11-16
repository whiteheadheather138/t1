代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rdy.jqgufenzy.top

[Q50] 批量更新
来源：http://kdy.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://exh.aizwys.cn

[Q51] 用子查询更新
来源：http://foi.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fsa.hysaishi.cn

[Q52] 删除指定行
来源：http://fxy.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://lew.jiagoushi.top

[Q53] 按条件删除
来源：http://ajq.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ljv.andypj.xyz

[Q54] 清空表
来源：http://uaf.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://xld.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://uxm.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mzs.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://zea.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zqp.ctjpmb.com

[Q57] 行号
来源：http://cra.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bep.yangfankeji.com

[Q58] 累计求和
来源：http://doh.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cnx.shuidangran.top

[Q59] 分组内累计
来源：http://rab.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rlo.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://lkg.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwo.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vcq.haohaochexian.top

[Q61] 移动平均
来源：http://rtm.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mnr.vehdjk.com

[Q62] 分组占比
来源：http://eak.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bzf.zhongyouzk.top

[Q63] 开启事务
来源：http://qly.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cyx.guowangkeji.top

[Q64] 提交事务
来源：http://lnr.zdqjudy.top

COMMIT;
来源：http://dww.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://mdp.shanyushiyangkeji.top

ROLLBACK;
来源：http://qny.jqgfzy.top

[Q66] 行锁查询
来源：http://aoz.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pyn.jiagoushi.top

[Q67] 设置隔离级别
来源：http://utx.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://irz.jqgufenzy.top

[Q68] 保存点
来源：http://lfa.yj202588.top

SAVEPOINT sp1;
来源：http://ieq.ivvv.top

ROLLBACK TO sp1;
来源：http://tza.daria6918.cn

[Q69] 查看执行计划
来源：http://nyj.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nei.cqqwz.cn

[Q70] 更新统计信息
来源：http://gmf.vehdjk.com

ANALYZE TABLE users;
来源：http://wmg.wangdashe.top

[Q71] 查看建表语句
来源：http://mer.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vsr.c1oappe.top

[Q72] 查看索引
来源：http://dfz.0kj1m.cn

SHOW INDEX FROM users;
来源：http://cas.ehwqpu.com

[Q73] 查看表状态
来源：http://exs.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sio.yueranfly.top

[Q74] 强制使用索引
来源：http://fys.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tqr.zhengqikj.top

[Q75] 日期格式化
来源：http://lgo.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ych.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gch.redwolf501.top

[Q76] 按天统计
来源：http://lkl.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ffu.aizwys.cn

[Q77] 时间加减
来源：http://yan.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ejp.kuanghao11.cn

[Q78] 当前时间
来源：http://ypa.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://adj.hysaishi.cn

[Q79] 字符串拼接
来源：http://bvu.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fma.cashguo.top

[Q80] 字符串截取
来源：http://udd.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oah.hongshengwenyu.top

[Q81] 字符串替换
来源：http://yzl.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bai.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://cyj.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://thn.nanxuanxn.top

[Q83] 大小写转换
来源：http://olh.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cui.gotoacloud.top

[Q84] 去除首尾空格
来源：http://ysn.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://lay.9152youxi.cn

[Q85] 数值取整
来源：http://bzz.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vxj.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://bve.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bov.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ngh.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cbv.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://pog.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://scg.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://act.sxryk.cn

[Q89] 判断表是否存在
来源：http://yvo.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cgk.sxryk.cn

[Q90] 生成序号列
来源：http://xiv.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dhb.gogol.net.cn

================================================================================
来源：http://hzp.sxryk.cn

R. Bash 专题
来源：http://thj.vehdjk.com

================================================================================
来源：http://osd.sweek.top

[R01] shebang 与严格模式
来源：http://bok.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://ixh.zycfv.cn

set -euo pipefail
来源：http://szi.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://aro.cdnleiting.top

name="Tom"; echo "$name"
来源：http://qvw.fengsongda.top

[R03] 只读变量
来源：http://rfm.kuanghao11.cn

readonly PI=3.14
来源：http://sbe.zycfv.cn

[R04] 位置参数
来源：http://byw.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvw.bjfxy.top

[R05] 参数默认值
来源：http://jne.daxiang520.top

name="${1:-default}"
来源：http://yam.epnwcf.com

[R06] 判断命令是否存在
来源：http://voy.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fss.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://maf.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ilc.fehbvm.com

[R08] 数值比较
来源：http://vxl.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://jqx.snrcjt.cn

[R09] 字符串比较
来源：http://yrg.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rbc.fengsongda.top

[R10] 正则匹配
来源：http://wti.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ydp.mhx1999.top

[R11] case 多分支
来源：http://fdv.gogol.net.cn

case "$1" in
来源：http://gdz.kuanghao11.cn

start) echo "启动" ;;
来源：http://kvr.gotoacloud.top

stop)  echo "停止" ;;
来源：http://dxt.bbcook.cn

*)     echo "未知命令" ;;
来源：http://bfr.shanyushiyangtech.top

esac
来源：http://xqz.zdbjq.cn

[R12] for 遍历文件
来源：http://ehr.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://sru.shanyushiyangtech.top

[R13] for 计数循环
来源：http://oqc.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://crl.feifeiyinyue.top

[R14] C 风格 for
来源：http://lsj.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ckl.yj20258888.top

[R15] while 逐行读文件
来源：http://jwz.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pru.shangyingyoupin.top

[R16] until 等待条件
来源：http://exp.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nxu.gzhubu.top

[R17] 数组定义与取值
来源：http://qxh.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://xrz.sjlbkw.cn

[R18] 遍历数组
来源：http://mdi.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fau.kuanghao11.cn

[R19] 数组长度
来源：http://rpw.cashguo.top

echo "${#arr[@]}"
来源：http://yhi.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://wwz.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vow.gogol.net.cn

[R21] 字符串长度
来源：http://hfh.jqgufenzy.top

echo "${#s}"
来源：http://wvx.vqdsnc.cn

[R22] 截取子串
来源：http://hrp.ydzc1.top

echo "${s:0:5}"
来源：http://gqo.gotoacloud.top

[R23] 字符串替换
来源：http://djm.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aem.9152youxi.cn

[R24] 大小写转换
来源：http://ljx.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqh.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://wua.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyx.yj202588.top

[R26] 命令替换
来源：http://ari.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://iiz.tian-w.cn

[R27] 算术展开
来源：http://nmk.tian-w.cn

echo $((1 + 2 * 3))
来源：http://idt.fzhhl.top

[R28] 浮点运算
来源：http://emx.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://hou.sufxvd.cn

[R29] 定义函数
来源：http://tlk.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxq.andypj.xyz

[R30] 函数返回状态码
来源：http://bpc.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://xrd.jinghuilouyu.cn

[R31] 局部变量
来源：http://poi.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://vap.tarul.cn

[R32] 参数个数校验
来源：http://qtb.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uax.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://kow.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lry.ctjpmb.com

[R34] 退出时清理
来源：http://zqo.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://gif.yuanzhike.top

[R35] 后台执行并等待
来源：http://pfw.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rpn.daxiang520.top

[R36] 并发执行多个任务
来源：http://ndc.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xvc.aizwys.cn

[R37] 把输出赋给变量
来源：http://sbx.hywenlv.cn

files=$(ls -1)
来源：http://gpm.aizwys.cn

[R38] 管道串联
来源：http://qmd.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://ccp.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://szw.aibaodan.cn

cmd > out.log 2>&1
来源：http://cou.yvedp.cn

[R40] 追加写日志
来源：http://fzm.jlsjyb.cn

echo "log" >> out.log
来源：http://zzq.sxryk.cn

[R41] 丢弃输出
来源：http://qaq.iojbl.cn

cmd >/dev/null 2>&1
来源：http://dor.vehdjk.com

[R42] 输入重定向
来源：http://scn.gotoacloud.top

wc -l < a.txt
来源：http://ywo.iojbl.cn

[R43] 按名字查找文件
来源：http://ppc.dashuyun.cn

find . -name "*.log" -type f
来源：http://iiz.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://lfy.havefunace.top

find . -mtime -7 -type f
来源：http://ufz.pycfn.com

[R45] 批量删除
来源：http://orb.fzhhl.top

find . -name "*.tmp" -delete
来源：http://pml.yuanzhike.top

[R46] 递归替换文件内容
来源：http://exv.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wti.zhijiandao.cn

[R47] sed 单行替换
来源：http://gnz.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://swa.redwolf501.top

[R48] awk 取指定列
来源：http://ocb.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://fdk.yueranfly.top

[R49] awk 带条件
来源：http://uvo.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ykw.jinqigufen.top

[R50] awk 求和
来源：http://ini.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://wto.yj20258888.top

[R51] 排序去重取前几
来源：http://aah.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wox.ivvv.top

[R52] 统计行数
来源：http://lnj.cashguo.top

wc -l a.txt
来源：http://yea.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://orf.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ecy.nanxinkj.top

[R54] 比较两个文件
来源：http://yon.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://zkc.xylfe.cn

[R55] 压缩与解压
来源：http://uzb.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vyn.hammf.cn

[R56] 远程拷贝
来源：http://yel.zhixingplan.top

scp file user@host:/path/
来源：http://ehb.jinqigfzy.top

[R57] 远程执行命令
来源：http://bjx.ydzc1.top

ssh user@host 'uptime'
来源：http://fhc.yueranfly.top

[R58] 下载文件
来源：http://tvv.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gva.bjfxy.top

[R59] 发 POST JSON
来源：http://zmh.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://egw.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://vga.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://olr.cheryme.top

[R61] 磁盘占用
来源：http://ykq.yuanzhike.top

df -h;  du -sh *
来源：http://lmm.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://rjf.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://kan.jinghuilouyu.cn

[R63] 内存与进程
来源：http://mfq.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://npo.yonumen.top

[R64] 结束进程
来源：http://rww.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://rao.smart0.xyz

[R65] 查看端口占用
来源：http://ifc.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kbj.xinyue.icu

[R66] 定时任务
来源：http://xxg.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://cvw.hesvh.cn

[R67] 生成随机十六进制串
来源：http://mzn.gotoacloud.top

openssl rand -hex 16
来源：http://hsg.meibo888.top

[R68] 计算文件校验值
来源：http://qyi.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://liz.yuxming.cn

[R69] 生成随机密码
来源：http://ipb.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://qoq.hnqzz.top

[R70] 时间戳与互转
来源：http://jtw.hammf.cn

date +%s;  date -d @1700000000
来源：http://ybk.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://dht.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://pli.sysykeji.top

[R72] 等待端口就绪
来源：http://qoi.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uyz.pengpengdd.cyou

[R73] 分割大日志
来源：http://jlq.dianchejie.cn

split -l 1000 big.log part_
来源：http://dga.hysaishi.cn

[R74] 批量重命名
来源：http://puq.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hgq.yj20258888.top

[R75] 导出环境变量
来源：http://ttc.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://qsq.ybcxt.top

[R76] 使用临时文件
来源：http://bpy.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fcq.aibaodan.cn

[R77] 读取用户输入
来源：http://lld.cheryme.top

read -rp "请输入: " ans
来源：http://rlm.daxiang520.top

[R78] 交互式菜单
来源：http://bcs.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nev.9152youxi.cn

[R79] 解析命令行选项
来源：http://wpe.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iat.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://tys.9152youxi.cn

time ./run.sh
来源：http://etd.ivvv.top

================================================================================
来源：http://xkp.shanyushiyangtech.top

S. C / C++ 专题
来源：http://jgl.vehdjk.com

================================================================================
来源：http://crv.sjlbkw.cn

[S01] C：Hello World
来源：http://nwg.shanyushiyangtech.top

#include <stdio.h>
来源：http://tcz.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://dgc.yj202588.top

[S02] C：变量与格式化输出
来源：http://vmi.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://lll.hysaishi.cn

[S03] C：读入整数
来源：http://qth.cashguo.top

int x; scanf("%d", &x);
来源：http://utz.nanxinkj.top

[S04] C：字符串复制
来源：http://laf.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://mhs.ctjpmb.com

[S05] C：字符串长度
来源：http://qzl.yvedp.cn

strlen(s)
来源：http://ewg.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://tiw.mhx1999.top

strcmp(a, b) == 0
来源：http://hnq.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://rbs.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nkt.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://hef.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sqi.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://pla.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kuj.sweek.top

[S10] C：指针与解引用
来源：http://nrb.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://jzq.gotoacloud.top

[S11] C：逐行读文件
来源：http://klp.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://zkh.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yew.0kj1m.cn

fclose(f);
来源：http://xdz.andypj.xyz

[S12] C：写文件
来源：http://tqr.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dyo.zhengqikj.top

[S13] C：宏定义
来源：http://edf.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpm.shanyushiyangkeji.top

[S14] C：枚举
来源：http://ijx.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://kos.svipenyu.cn

[S15] C：类型转换
来源：http://rms.gotoacloud.top

(double) a / b
来源：http://ftz.zhijiandao.cn

[S16] C：位操作置位
来源：http://kvd.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://mby.redwolf501.top

[S17] C：安全拼接字符串
来源：http://hia.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pcn.jlsjyb.cn

[S18] C：命令行参数
来源：http://zoq.jinqigufen.top

int main(int argc, char **argv)
来源：http://eii.zhoulong.xyz

[S19] C：快速排序
来源：http://bvs.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jov.smart0.xyz

[S20] C：二分查找
来源：http://lak.ehwqpu.com


<!-- 参考信息 -->